## Data model

We'll have the following entities:

|`User` table|
|--|
user\_id (PK)
name
email

|`Questions` table|
|--|
question\_id (PK)
path\_to\_content\_file
path\_to\_test\_cases\_file
path\_to\_solutions\_file

|`UserSubmissions` table|
|--|
user\_id (FK)
submission\_id (PK)
question\_id (FK)
submission\_timestamp (indexed)
path\_to\_code\_contents
status (`PENDING`, `ENQUEUED`, `WRONG_ANSWER`, `ACCEPTED`, `TLE`, ...)
last\_update\_timestamp


