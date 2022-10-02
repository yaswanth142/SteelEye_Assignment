# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)

//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

### 1)Explain what the simple List component does.
### 2)What problems / warnings are there with code?
### 3)Please fix, optimize, and/or modify the component as much as you think is necessary.

### Answer 

### LISTS:

->Lists are used to display data in an ordered format and mainly used to display menus on websites. 
->In React, Lists can be created in a similar way as we create lists in JavaScript. 

### List Compounent and Example:

->In React, Lists can be created in a similar way as we create lists in JavaScript.
-> Let us see how we transform Lists in regular JavaScript. 
->The map() function is used for traversing the lists. 
->In the below example, the map() function takes an array of numbers and multiply their values with 5.

### Errors in Code:

### Step1:

### Error1:

  onClick={()=>onClickHandler(index)}

  OnClick is an functional Component ,so we can used the {()=>} Arrow Function

### Error2:

   index: PropTypes.number
In this ,We are not added the index ,Index is used to taken the parent component and indentify the unique value and varables.
Maping the indexes,we use the index on return function

### Error3:

  const [setSelectedIndex, SelectedIndex] = useState();

  ->In the above code having error ,Because the error is in the the position of the data and setdata are interchanged so, 
  ->we have to retify the error in the useState hook

  const [selectedIndex, setSelectedIndex] = useState();

### Error4:
   
   Use the arrayof instead of array and Shape instead of shapeof in the WrappedListComponent.propTypes 

### Error5:
  
    We have to pass the data using props 

WrappedListComponent.defaultProps = {
  items: null,
};

After Retifying Error,

WrappedListComponent.defaultProps = {
  items: [{text:"yeswanth",index:1}],
};



