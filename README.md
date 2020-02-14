# AdamandAntoniaEngWeek
In this folder you'll find a app.py file with our API, and a simple database in JSON.

In this project, we built a data API that will help us store and retrieve posts from our journal. It is built in Python, using a framework called Flask. We deploy our API using https://www.pythonanywhere.com/ , which allows us to publicly deploy our API to be called. 

## Restful API Supporting diary:

| Route        | Method | Use                          | Arguments | Returns                                                                                                                                                                               |
|--------------|--------|------------------------------|-----------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| /diaryentry  |   GET  | Bring back all diary entries | None      | string containing dictionary of unique ids and diary entries response = {"success_message": "We've found your diary entry!", "returned_entry": returned_entry, "entry_id": entryid, } |
| /diaryentry  |  POST  | Create a new diary entry     | Takes a single argument as 'diary entry', retrieved by request.data json.loads(request.data)    | response = {,"message": "New entry created",,"data": diary_entry,,"id": unique_id,}                                                                                                   |
| /diaryentry/<entryid> |   GET   |  Not in use as under development. Gets a single diary entry   |           |                                                                                                                                                                                       |
