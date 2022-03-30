# Optimizeapp React Native Challenge

## Introduction

At OptimizeApp we spend all day figuring out how to get customers ads online as quickly and easily as possible. As a front end developer, you have to build UI/UX to streamline our customer experience and functionality. Your task here is to design 4 simple screens to check the functionality of form submission, using a GET request to display JSON data, and navigating between said screens.

## Requirements

1. We value a **clean**, **simple**, working solution.
2. Candidates must submit the project as a git repository. The repository must avoid containing the words `optimizeapp` and `challenge`.
3. Application should run on both iOS and Android.

## Assignment tasks

1. Create 4 screens that can be navigated between all of them
2. First screen is a main Home Screen that contains 1 button that navigates to campaign creation screen and another button that navigates to campaign detail screen)
3. Campaign creation

   - First screen
     - Ability to write and set the name for the campaign
     - Ability to choose an objective(i.e. options) from a list (website or brand_awareness)
     - Ability to submit the data to an api endpoint and passing the response data to the next screen (i.e. the campaign id, name and objective from the response)
     - API : POST https://www.optimizekwtestingserver.com/testdemo/public/campaign
            Params: {name: "test campaign", objective: "BRAND_AWARENESS"} 
   - Second Screen
     - Display the campaign name
     - Ability to choose a media file to be uploaded, should be restricted to a 9:16 aspect ratio and minimum resolution of 1080x1920
     - Based on the objective that was returned from the response in the previous screen there should be a field to enter a url if the objective was website or not if it's brand awareness. (Bonus if there is url validation)
     - Ability to submit the data to an api endpoint and return back to the Main Screen.
      - API : POST https://www.optimizekwtestingserver.com/testdemo/public/creative
            Params: {name: "test campaign", website_url: "https://www.optimizeapp.com", media: FILE Object} 

4. Campaign details
   - Make a GET request to an API endpoint and retrieve a JSON data object
     - Display said data to fill in and design the detail screen including a graph/circle bar to show how much was spent from the lifetime budget
     - API: GET https://www.optimizekwtestingserver.com/testdemo/public/campaigndetail/2238


- Fonts and colors are to be used from the Assets folder
- For the icons you can use any free website that provides icons like https://oblador.github.io/react-native-vector-icons/
- The required libraries to be used in this assignment are: react-navigation v4, Axios for api requests and Redux for actions and reducers
- Feel free to use any other libraries that might help you with the tasks

## Bonus Tasks

1. Having UI tests is a strong bonus.

Questions? We love to answer: admin@optimizeapp.com
