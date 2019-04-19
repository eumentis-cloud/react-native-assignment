# Eumentis Cloud - React Native assignment

Here we provide the instructions for developing an android app with React Native, designed by the Eumentis Cloud team, to test the proficiency of applicants for the React Native Frontend Developer position(s).

## Prerequisites
* Knowledge of React & React Native
* Knowledge of installing npm packages (both local & global)
* Knowledge of fetching JSON data from a REST API endpoint
* A Github account in order to share his/her code with us

## Submission guidelines

All applicants must submit the code and the release APK file (Android) for evaluation.

### Sharing the code

The complete React Native assignment code should be uploaded to a public repository on your Github account.

### Sharing the android release APK file

An APK file should be generated and uploaded to [Diawi](https://www.diawi.com/).

### Submission
The link to the Github repository and the Diawi link (of APK file) should be submitted by filling out the following form:

[https://forms.gle/F7B2hFY3Nwp9KSVA8](https://forms.gle/F7B2hFY3Nwp9KSVA8)

## Assignment Details

**Deadline for submission:** 5 days

The aim of the assignment is to build an android app that shows the basic details of 10 users' profile data (the data is obtained from an API endpoint). Each user's profile information is displayed in a card and the app will show a scrollable list of all the 10 cards.

Each card displays the user's picture, name, email, dob & mobile no. At the bottom of each card there is a section related to voting each user. It contains buttons to upvote and downvote a user and the current live vote count is also displayed.

The user profile cards are sorted by the no. of votes in descending order (user with highest vote is displayed at the top and the one with lowest is displayed at the bottom).

#### Assignment Demo
 
We have created a working demo of the assignment for applicants to refer to. All applicants are requested to create an exact replica of the demo app.

[Link to demo APK file](https://1drv.ms/u/s!AqkRCvgUCZensGHu08vREO0R-rh9?e=vgWJAr)

[Link to the video demonstration of the app](https://youtu.be/IMob6bNdpV0)

#### API endpoint for users data

All 10 users profile data is to be downloaded from the following API endpoint:
```
Method: GET
URL: https://randomuser.me/api/?results=10&seed=eumentis
```

The schema of the data received in the response is:
```Javascript
{
  results: [
    {
      // Full name is displayed in the user's profile card
      name: {
        first,
        last,
      },
      email,
      login: {
        // The id for each user
        uuid: "c4168eac-84b8-46ea-b735-c9da9bfb97fd",
      },
      dob: {
        date: "1975-11-12T06:34:44Z",
      },
      // User's mobile no.
      cell,
      picture: {
	// The URL for user's profile picture
        large,
      }
    }
  ]
}
```

#### Icons

All the icons in the apps were added using the following package:
[react-native-vector-icons](https://github.com/oblador/react-native-vector-icons)

### UI Design

The following picture describes the different colors used in the app & the user card.

![UI design of cards - colors](https://9auhoa.bn.files.1drv.com/y4m0GZMYYj3v30Xeb1MPA-8a40CkhBF0hsX301OVG_3kJgF44kW8Zyys-zEcUgfDXElLS1J3S-jNIGiqFjiQYQgH32VvGfZ_7UW-Cczaa0gwqHtB4yk-iDT91Onqp7ct7OkUqp7AQzAB8b0zILlIydkZeT0zQ87Z4pM9yBqLdXuVC3gZU0kpINYs8njbNJwBFlDG7SOs4Dx0e5JpfI4VMKd_A?width=1024&height=643&cropmode=none)

## Things to note in the demo application

### Loading indicator

As soon as the app opens a loading indicator is shown until the users data is fetched.

### Toast message

A toast message (at the bottom of screen) is shown when the user data is fetched from the API. The message shown is: `Users download complete!`

## General Tips

 - Feel free to use Google, StackOverflow or any other resource
 - Examine the demo apps closely to determine all the features
 - Open the data API link in your browser/Postman and examine the response schema
 - Try to match the UI design of the demos for each assignment as closely as possible.
 - Please feel free to get in touch with the Eumentis Cloud's team to clear any doubts related to the aforementioned instructions.
