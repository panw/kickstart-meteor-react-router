# kickstart-meteor-react-router

Kickstart a project with Meteor, React and react-router fast!

1. git clone https://github.com/thereactivestack/kickstart-meteor-react-router.git
1. cd kickstart-meteor-react-router
1. meteor
2. npm install
3. meteor

# Production
You can use meteor run, meteor build, mup or anything working with Meteor.

## Run in production mode
`meteor run --production`

## Build for production
`meteor build .`

# Cordova
You need to do those 3 steps to make it works with iOS or Android:

1. Add the platform to your Meteor project

    ```javascript
    meteor add-platform ios
    meteor add-platform android
    ```
1. Allow access to your dev server in your `/mobile-config.js` file:

    ```javascript
    App.accessRule('http://192.168.1.100:3500/*');
    ```

1. Replace localhost by your local ip address in `webpack.json`.
