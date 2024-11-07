# Kanya Srithong
Design for the soul

Check out some of my work below

# I’m Kanya, nice to meet you!

I’m a Philadelphia-based undergraduate student studying **User Experience and Interaction Design (UXID)** at **Drexel University**. I’m also currently working as a **Web Content Editor** for Drexel’s Office of the Provost. I’m seeking to expand my knowledge on **product design**, **graphic design**, **user research methodologies**, and **frontend development**. Through my work, I hope to bridge the gap between aesthetic sensibilities and more accessible, user-friendly digital interfaces!

Aside from my design and development work, I love to **crochet** 🧶, **do puzzles** 🧩, **explore the city with friends** 🌆, and **play the flute** 🪈!


# Drexel Scheduler Redesign
## Overview 

During my Introduction to Human-Computer Interaction course, I worked with three groupmates on a usability evaluation of our chosen interface. In our case, this was a website created by a Drexel undergraduate combining data from Drexel’s Term Master Scheduler with the website Rate My Professor to help aid students in the class scheduling process. Through the gathering of user feedback, collaboration, and our knowledge of Don Norman’s principles, we each created wireframes using Draw.io detailing proposed changes to the user interface.

## The Problem

The Drexel Scheduler had issues with its overall layout, information hierarchy, and confusing signifiers. Users had difficulty when it cames to navigating certain elements of the user interface, such as the central table containing information about each class and the corresponding professor as well as its accompanying search filters. Because the creator’s intentions were to move the website from its original platform onto a custom domain and redesign it from the ground up, he requested for my group to provide user experience-related feedback to aid him in this process.

## Goals

Overall, my group’s goals for this redesign were to:
1. Create wireframes that both improve the layout of the website to better utilize whitespace
2. Highlight changes that can be made to certain UI elements to improve their usability

## Design Process:
### Research:

As part of the target audience for this product, students who attend Drexel University required to schedule our own classes for each term, my group took it upon ourselves to identify the pain points of the original interface. After creating individual wireframes recreating the structure and components page, mine shown below, we came together to discuss our findings.


After our discussion, we made the decision to each create our own wireframes illustrating proposed changes we would make to resolve pain points we each identified, with the intention of increasing the website’s overall usability. I then connected my proposals to the design principles Don Norman outlined in his book *The Design of Everyday Things*, my focal point being the search filters used to narrow down the results of both the entire table and the individual columns within: 

### Change #1: Visibility
#### Original

At first glance, the overall visibility of the Drexel Scheduler website was quite overwhelming to look at, with the multiple sections and confusing layout preventing a clear focal point for the viewer to be drawn to. The main culprits perpetuating this issue was the table-wide filters above the table, which took up an unnecessary amount of space at the top of the screen. 

#### Redesign

Because the scheduler table should be the main focal point of the interface, I condensed the table-wide filters into a “Filter” button located at the top right of the scheduler table in order to prioritize the table’s visibility. This feature also allows the user to adjust the visibility of these filters to their own liking. 

When the filter button itself is clicked on, a main dropdown menu becomes visible with the previous filters being sorted into a number of sections that act as category-specific dropdowns: the “Course Number” category containing filters related to the Course Number column in the table, the “Instructor Information” category pertaining to filters altering columns related to Rate My Professor data, and the “Times” category containing filters associated with the course time-related columns. 

Additional filters that do not fall within these categories are located in a separate section at the bottom of the dropdown. To improve the visibility of this Filter section, category names are bolded and the filters are white in order to make them stand out against the background. 

### Changes #2 & #3: Constraints & Affordances
#### Original

The original interface contained filters for each individual column in the main table. As seen in the image above, when attempting to utilize the search bar filter within the individual column filter, the word “Contains”, inequality symbols, and the word “Expression” are given as options. The word “Contains” would be relevant to include, as selecting that option implies that the results that show up would contain the user-inputted text. The inclusion of the inequality symbols as options, however, were not applicable to the filtering of non-numerical values and yet still appeared for such filters, demonstrating the lack of a constraint. As to the usage of “Expression”, the functionality of this option was also unclear. Within my personal evaluation, the inclusion of these options only served to confuse me, causing a disruption to my ability to perform my task. 

Also shown in the top right of each image is the “Match Case” button, a feature that allows the user to specify whether the case of the text input to the search bar affects the search results. In my initial evaluation of the interface, I had not taken note of this feature as an affordance, as it was placed above the search bar away from the other search filters. My personal mental model saw such a feature as being in a spot that would make it more noticeable such as the search bar, and this was not reflected in the original design.

#### Redesign

The images above present a wireframe aiming to constrain the search filtration feature to basic, user-friendly components. It removes the inequality symbols and “Expression” options, and presents two options for the search filter dropdown: “Contains” and “Does Not Contain”. The utilization of these phrases makes it clear to the user their usage: “Contains” serves the function stated previously while “Does Not Contain” shows the options that do not include the user-inputted text.

This change not only simplifies the process for the user in terms of understanding the functionality, but also works to prevent the possibility of the user misusing options that are irrelevant to the type of data presented. 

This wireframe reflects a modification to the feature that relocates it to be a part of the search bar. The choice to move the “Match Case” button to the search bar, the location that is being affected by its function, helps to better communicate to the user its functionality. Additionally, a gray box is added onto the button to help better distinguish the feature as a button rather than a design choice added purely for aesthetic reasons, which was my initial interpretation in the original interface.

## Results

My group presented our findings and proposals to our classmates, professor, and the student who developed the website, Zohair Ul Hasan. Zohair was grateful for our input, and commented on how he plans to take into account our feedback within his website redesign. In addition to our presentation, we wrote papers expanding upon our individual feedback that were given to the professor. This class, along with this project, allowed me to gain an intensive understanding of the process of implementing effective, user-friendly changes to a user interface. 

# Spotify Record Player
## Overview
For my Maker Workshop class, we were given the task of creating an object utilizing 3D printed components designed using CAD software and an Arduino UNO with functioning code in C++. Utilizing the Spotify API, I altered a Python script that extracts the song name and artist of the current track playing on my personal Spotify account, which were then displayed on an LCD screen connected and powered by my Arduino. The LCD Screen and Arduino components were then encased in a 7” x 7.5” inch 3D printed shell modeled in TinkerCAD to resemble the shape of a record turntable.

## Brainstorming Phase
I had come up with a number of initial ideas, a list of which is shown below:

Out of all of these, the record player idea appealed to me the most. I thought that it would be a good way to challenge myself with this project and allow me to utilize some of my Python knowledge. 

## Programming & Debugging Phase
I first researched methods of extracting specific data from a Spotify account, in this case my own, and allow it to be processed through the Arduino. My initial search led me to a tutorial detailing how an individual went about this exact task using Python and C++ within the official Arduino IDE. My recreation and tests of both the wiring and the provided source code on their GitHub, however, led me to realize that much of the information turned out to be outdated. After much time spent attempting to debug and update the program, I soon realized that finding an alternative method would end up being less time consuming in the long run.

Fortunately, I stumbled across another GitHub page detailing how to go about the task through the use of Spotify’s Web API in addition to the previously mentioned programs. After creating my own Spotify for Developers account and creating an application to reference within my Python program, I once again debugged and updated other necessary aspects of the program in order for it to function properly.

## Assembly Phase
Utilizing models I had found for parts of a miniature record player, I modified them using TinkerCAD to both be larger than the original size and to have a hollow base in order to accommodate the Arduino, all of which were eventually printed using a MakerLab 3D Printer. I had initially added a hole in order to accommodate a motor to spin the record plate, however this did not pan out in the printing process and the idea was scrapped. As for the Arduino wiring, I condensed wiring I had taken from the original tutorial I had found onto a smaller breadboard in order to fit within the hollow base. 

## Results
Although the programming phase was incredibly arduous, showcasing the final product to the class and professor was worth the effort put into the project. Online resources, my knowledge of Python from a previous Computer Science class, and my own creativity were integral in my success. This class not only fueled a child-like sense of product design creation for me, but also allowed me to develop a better understanding of the design process and the utilization of different tools like laser cutters, basic CAD software, and Arduino!

**Watch the Spotify Record Player at work!**

Check out some of my creative work here, which includes a mix of **drawing**, **painting**, **design work**, and **photography**! 

