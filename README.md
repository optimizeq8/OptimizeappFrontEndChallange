# Optimizeapp React Native Challange

## Introduction

At OptimizeApp we spend all day figuring out how to get customers ads online as quickly and easily as possible. As a front end developer, you have to build UI/UX to streamline our customer experience and functionality. Your task here is to design 4 simple screens to check the functionality of form submission, using a GET request to display JSON data, and navigating between said screens.

## Requirements

1. We value a **clean**, **simple**, working solution.
2. Candidates must submit the project as a git repository. The repository must avoid containing the words `optimizeapp` and `challenge`.
3. A screen recording of the application should be attached in the repository.

## Assignment tasks

1. Create 3 screens that can be naviagted between all of them
2. Campaign creation

   - First screen (reference: [here](https://github.com/optimizeq8/OptimizeappFrontEndChallenge/blob/main/Screen%20Templates/Campaign%20Creation%201.png))
     - Ability to write and set the name for the campaign
     - Ability to choose an objective (website and brand_awareness) from a dropdown-list (Bonus: Make it similar to the design [here](https://github.com/optimizeq8/OptimizeappFrontEndChallenge/blob/main/Screen%20Templates/Campaign%20Creation%201%20objectives.png))
     - Ability to submit the data to an api endpoint and save the response data (i.e. campaign name and objective) in a redux store, use that data on the next screen 
     - API : POST https://www.optimizekwtestingserver.com/testdemo/public/campaign 
       - Params: {name: "test campaign", objective: "BRAND_AWARENESS" OR "WEBSITE"} 
   - Second Screen(refrence: [here](https://github.com/optimizeq8/OptimizeappFrontEndChallenge/blob/main/Screen%20Templates/Campaign%20Creation%202.png) and [here](https://github.com/optimizeq8/OptimizeappFrontEndChallenge/blob/main/Screen%20Templates/Campaign%20Creation%202%20with%20media.png))
     - Display the campaign name
     - Ability to choose a media file to be uploaded. (Bonus : Media should be restricted to a minimum resolution of 1080x1920)
     - Based on the selected objective in the previous screen, if the objective was "WEBSITE" a field should be shown to enter a website url (Bonus if there is url validation), or do not show the website feild if the objective is BRAND_AWARENESS.
     - Ability to submit the data to an api endpoint and navigate to the Campaign details Screen.
     - API : POST https://www.optimizekwtestingserver.com/testdemo/public/creative 
       - Params: {name: "test campaign", website_url: "https://www.optimizeapp.com", media: FILE Object}
     
3. Campaign details (reference: [here](https://github.com/optimizeq8/OptimizeappFrontEndChallenge/blob/main/Screen%20Templates/Campaign%20Detail%20Screen.png))
   - Make a GET request to an API endpoint and retrieve a JSON data object
     - Display said data to fill in and design the detail screen. (Optional: Ad Performnace section)
     - API: GET https://www.optimizekwtestingserver.com/testdemo/public/campaigndetail/2238
- Feel free to follow the screen templates as design references or use your own designs
- Fonts and colors are provided from the Assets folder
- For the icons you can use https://oblador.github.io/react-native-vector-icons/
- The required libraries to be used in this assignment are: Native-Base for icons, react-navigation, Axios for api requests and Redux for actions and reducers
- Feel free to use any other libraries that might help you with the tasks

## Advantageous Bonus Task

1. Having UI tests is a strong bonus.

Questions? We love to answer: admin@optimizeapp.com
