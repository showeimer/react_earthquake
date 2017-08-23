# Earthquakes - Simple React App
Build a simple React application using create-react-app and scaffold the project with separate components and styles folders.

The design of a React application is important from the structure to the code. We scaffold our projects to help separate the various pieces of the application we create and organize the pieces to fit together. As the complexity of our application increase so too does the need for organization of our project.

## To get started, complete the following tasks:

Create a folder called components inside of your src directory for project files.

Create a folder called styles inside of your src directory for style sheets.

In the public directory, open the index.html file and add the following <link> tag under the last link in the '<head>' : '<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-alpha.6/css/bootstrap.min.css" integrity="sha384-rwoIResjU2yc3z8GV/NPeZWAv56rSmLldC3R/AZzGRnGxQQKnKkoFVhFQhNUwEyJ" crossorigin="anonymous">'

Add a class of container-fluid to your '<div id="root"></div>' in your index.html.

Move your App.js file in to your components folder.

In your index.js file, change the file path for your App.js importing of your App component to the correct file path.

Move your index.css and your App.css files into your styles folder.

In your index.js file, change the file path of your index.css import to the correct path name so they are properly linked.

In you App.js file, change the file path of your App.css import to the correct path name so they too are properly linked.

In the App.css file, copy and paste the starter App.css from the starter_files over all existing CSS.

Delete the logo.svg import statement from your App.js file.

Delete the entire '<div className="App-header">' from your App.js file.

Create a '<div className="title">' inside of your .App div in your App.js file.

Create a '<div className="my-header">' in your App.js file inside of your .title div and type "Earthquakes!" inside of it to make sure everything is linked up properly.

Create a folder called data in your src directory.

Create a file called earthquakes.js in your data folder.

Copy the code from the earthquake.js file in the starter_file folder into your own earthquake.js file.

## Creating the Project  

You will need to create the following components and import them and nest them properly in your App.js file and component.

An EarthquakeList.js file with an EarthquakeList component.

The EarthquakeList component should be exportable.

You should add import moment from 'moment'; underneath you import statement for React.

You will need to import your earthquake data from your data folder as earthquakes. SEE HINTS.

You should create an EarthquakeInfo.js file with an EarthquakeInfo component.

The EarthquakeInfo component should be exportable.

The EarthquakeInfo should render a single div with the class "earthquake-title" to match the class in the style sheet. The div should include the following text: "This is a list of 8 Earthquakes occurring on the morning of July 14th across the United States."

Underneath the .title div you should place the EarthquakeInfo then the EarthquakeList components.

### Hints  

Inside of the render method, map over your data and return the following '<div>'.

<div className="col-sm-6" key={FILL_ME_IN_WITH_A_UNIQUE_KEY}>

  <div className="card" >

    <div className="card-block">

      <h4 className="card-title">{FILL_ME_IN_WITH_THE_PLACE}</h4>

      <h6 className="card-subtitle mb-2 text-muted">Magnitude: {FILL_ME_IN_WITH_THE_MAGNITUDE_MAG}</h6>

      <h6 className="card-subtitle mb-2 text-muted">Time: {moment(FILL_ME_IN_WITH_THE_TIME).format('llll')}</h6>

      <p className="card-text">Coordinates: {FILL_ME_IN_WITH_THE_COORDINATES}</p>

      <a href={FILL_ME_IN_WITH_THE_URL} className="card-link">USGS Event Link</a>

    </div>

  </div>
</div>

The above div should be returned from a map function into the following div:

<div className="quake-list">

  <div className="row">

    {quakes}

  </div>

</div>

Be sure to use the mock up below to check your work and see if you are putting together your application correctly.
