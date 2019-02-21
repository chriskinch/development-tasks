React with REST data
==========

This example assumes that you have a basic understanding of the React library and is intended to probe your knowledge of component structure, basic routing, API calls, simple styling methods and testing methods.
You should aim to spend approximately 2 to 3 hours on this exercise.


## Task

We are going to set up a single page React application that consumes data via a REST API and displays that data on the page using components.
The data will come in the form of a list of photos, those should be grouped by album.
A user should be able to navigate to view albums and photos without additional API calls. 


## Technical details

The REST API that we are using for this example is from: https://jsonplaceholder.typicode.com  
The particular endpoint that should be called is: `https://jsonplaceholder.typicode.com/photos?_limit=300`

The project should be executed with the following commands:

`npm install` for project dependencies.  
`npm start` for a local development preview.  
`npm run test` for local unit testing which must pass.

I would recommend using a toolchaing such as https://github.com/facebook/create-react-app as this exercise is not design to test you build configuration knowledge.


## Acceptance criteria

- Photos should be limited to 300 items.
- The album list should display:
  - A heading as `Album [albumId]`
  - A thumbnail of the first photo within the album
- The photo list should display:
  - A heading as `[title]`
  - A thumbnail
- Any unit tests included should pass


## Stories

### Application entry

    As a user
    When I land on the entry point of the application
    A list of albums should be displayed

### Navigation

    As a user
    When I click on an album
    I should see a list of photos from that album
    
    As a user
    When I click on a photo
    I should see a larger representation of that photo only

### Layout

    As a user
    When I browser albums or photos
    I should see items displayed in a responsive 6 column grid
