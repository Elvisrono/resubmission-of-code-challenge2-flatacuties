# Flatacuties
This is an app for building and voting for the cutest animal.
# Development requirements
- Visual studio code
- Live server  extension
- npm
- json-sever
# Development
To get the code,
```bash
 click on this link: https://github.com/kericho/code-challenge2flatacuties.git
 ```
- fork and git clone the code to you local machine.
- Navigate to this folder by running this command:
```bash
 cd code-challenge2flatacuties/
 ```
- open the code using this command, 
```bash
   code .
```

- run this command on your terminal:
```bash
 json-server --watch db.json.
 ```
- Below at the bottom of your vs code click on the Go live to display the animals on the browser
# Technology used
- HTML
- CSS
- Javascript
- Bootstrap

# Deliverables

As a user, I can:

1. See all characters names in a `div` with the id of `"character-bar"`. Create
   a `span` tag with the character's name and add it the `div#character-bar`
   once you have retrieved the character data from the server. You will need to
   make a GET request to the following endpoint to retrieve the character data:

   ```txt
   GET /characters

   Example Response:
   [
    {
      "id": 1,
      "name": "Mr. Cute",
      "image": "https://thumbs.gfycat.com/EquatorialIckyCat-max-1mb.gif",
      "votes": 0
    },
    {
      "id": 2,
      "name": "Mr. Monkey",
      "image": "https://thumbs.gfycat.com/FatalInnocentAmericanshorthair-max-1mb.gif",
      "votes": 0
    },
    ...
   ]
   ```

2. When the character in the `div#character-bar` is clicked, display the
   character's details in the `div#detailed-info`. You can either use the
   character information from your first request, or make a new request to this
   endpoint to get the character's details:

   ```txt
   GET /characters/:id

   Example Response:
   {
    "id": 1,
    "name": "Mr. Cute",
    "image": "https://thumbs.gfycat.com/EquatorialIckyCat-max-1mb.gif",
    "votes": 0
   }
   ```

3. When the `form#votes-form` is submitted, add the number of votes from
   the input field to the character displayed in the `div#detailed-info`. **No
   persistence is needed**.



    ```txt
    POST /characters

    Request Headers: {
      Content-Type: application/json
    }

    Request Body: {
      "name": "Character Name",
      "image": "https://example.com/my-image.gif",
      "votes": 0
    }

    ----

    Example Response: {
      "id": 6,
      "name": "Character Name",
      "image": "https://example.com/my-image.gif",
      "votes": 0
    }
    ```
