In this project, I built a **CCBP Timeline** by applying the concepts I have learned till now.

### Refer to the image below:

<br/>
<div style="text-align: center;">
    <img src="https://assets.ccbp.in/frontend/content/react-js/ccbp-timeline-output.gif" alt="ccbp timeline output" style="max-width:70%;box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12)">
</div>
<br/>

### Set Up Instructions

<details>
<summary>Click to view</summary>

- Download dependencies by running `npm install`
- Start up the app using `npm start`
</details>

### Completion Instructions

<details>
<summary>Functionality added</summary>
<br/>

The app have the following functionalities

- Initially, the page display's the timeline items list using **Chrono custom rendering** based on the `categoryId`
- The `TimelineView` component is provided with `timelineItemsList`. It consists of a list of timeline item objects with the following properties in each timeline item object

  - The timelineItemObject with `categoryId` as `COURSE` have the following properties

    | Key         | Data Type |
    | ----------- | --------- |
    | id          | String    |
    | categoryId  | String    |
    | title       | String    |
    | courseTitle | String    |
    | description | String    |
    | duration    | String    |
    | tagsList    | Array     |

  - The tagsListObject will have the following properties

    | Key  | Data Type |
    | ---- | --------- |
    | id   | String    |
    | name | String    |

  - The timelineItemObject with `categoryId` as `PROJECT` have the following properties

    | Key          | Data Type |
    | ------------ | --------- |
    | id           | String    |
    | categoryId   | String    |
    | title        | String    |
    | projectTitle | String    |
    | description  | String    |
    | imageUrl     | String    |
    | duration     | String    |
    | projectUrl   | String    |

- If the value of the key `categoryId` in timelineItemObject is `PROJECT` then Project card will rendered
  - The Project card consist of **Visit** link when a user clicked on it, then the page will be navigated to the respective project
  - The Project card consist of a **Clock** icon with respective `duration` text
- If the value of the key `categoryId` in timelineItemObject is `COURSE` then Course card will be rendered
  - The Course card consist of a **Calendar** icon with respective `duration` text
- Given the timeline items list data as a `items` prop for the Chrono component from **react-chrono**, so that the title will be displayed beside each card

</details>

