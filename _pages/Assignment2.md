---
permalink: /Assignment-2/
title: "Assignment-2"
---

                 GROUP MEMBERS: Jane & Deema

# Mapping Houses in Oman from Lorimer’s Gazetteer

## 1. Choosing the topic

At the beginning of this project, we considered exploring religion in Lorimer’s Gazetteer. However, after examining several pages, we realized that religious information was not recorded consistently. Some entries mentioned several religious groups, while others included only one or two, making it difficult to identify meaningful patterns or collect comparable information. We therefore decided to focus on the number of houses recorded for different tribes. This information appeared more frequently throughout the Gazetteer and offered a clearer basis for comparison. We also chose to concentrate on Oman rather than covering a much larger geographical area, for this allowed us to work with a substantial amount of information while keeping the project manageable.

Our final dataset contains 108 records. Although this was below the approximately 300 points initially suggested for the assignment, we prioritized information that we could verify from the original source rather than including uncertain records simply to increase the dataset’s size. We also confirmed with the professor and he was okay with that.

## 2. Extracting and organizing the data

We used Gemini to assist with extracting information from Lorimer’s Gazetteer. Our initial prompt was based on a screenshot of Dhank Town, which recorded the number of houses associated with different tribes. We asked Gemini to create a table with Dhank Town as the first entry and a separate column for each unique tribe, adding the corresponding house counts. As we uploaded more screenshots, we adjusted the prompt to account for additional places listed under the column “Names”, repeated tribes across different settlements, and information mentioned in paragraphs accompanying the tables. We consistently instructed Gemini not to assume or invent information that was not explicitly stated in the screenshots.
The following is an example of the prompt we used and adapted as we continued uploading screenshots:

### “
This is a screenshot from Lorimer’s Gazetteer showing information about a place called Dhank Town, including the number of houses associated with different tribes. I want you to create a table starting with Dhank Town as the first row. For each unique tribe mentioned, create a separate column and enter the corresponding number of houses in the relevant cell.
We continued using this table as we uploaded additional screenshots. For the new screenshots, some information also appears under the column titled “Names”, which includes different places and settlements, even when the same tribes appear more than once. Please account for these different place names while keeping repeated tribal names consistent. Also, check any paragraphs accompanying the tables, as they may mention additional villages or settlements and their house counts.
<figure>
  <img
    src="{{ '/assets/images/image 1.png' | relative_url }}"
    alt="image 1"
    style="max-width: 100%; height: auto;">

  <figcaption>image 1</figcaption>
</figure>
 
 Include all relevant information in the existing table, adding rows and columns where necessary. Do not assume, estimate, or invent any information that is not clearly stated in the screenshots. If a detail is missing or unclear, leave the corresponding cell blank.
### ”

Our collection process involved using the geographical information available through Zenodo to identify places and their coordinates. We then searched for those places in Lorimer’s Gazetteer, examined their entries, and took screenshots whenever we found relevant information about houses and tribal affiliations. These screenshots were uploaded to Gemini for extraction.
One of our biggest challenges was deciding how to structure the information. Initially, we created a separate column for every unique tribe. However, as the dataset grew, this resulted in many empty cells because most settlements only contained information about a limited number of tribes. We eventually changed to a tidy table structure with a fixed set of columns: Place_Name, Region_or_Wadi, Tribe, Section_or_Subtribe, Houses, Structure, Shared_Tribe, latitude, and longitude, alongside a unique Row_ID.

Not every record included a clearly identified section or subtribe. In some cases, the Gazetteer mentioned the main tribe but did not provide further details. We decided to include these records in the dataset instead of excluding them, leaving the cells where the information was not available blank. This allowed us to retain useful information about settlements and house counts without making assumptions about subtribal affiliations that were not explicitly mentioned in the source. We also introduced the Shared_Tribe column, changing its original name from “Shared Count”. This column indicates whether a recorded house count belongs to one individual tribe or represents a combined figure shared between multiple tribes. This distinction helped us preserve the way information was presented in the original source rather than incorrectly attributing combined figures to individual tribes.

## 3. Visualizing the data with Kepler.gl

After cleaning and organizing the dataset, we exported it as a CSV and uploaded it to Kepler.gl.

<figure>
  <img
    src="{{ '/assets/images/image 5.png' | relative_url }}"
    alt="image 5"
    style="max-width: 100%; height: auto;">

  <figcaption>image 5</figcaption>
</figure>
 
We initially encountered difficulties with how the platform interpreted our data. Some fields were treated as numerical values, causing Kepler.gl to display averages or “NA” instead of the information we wanted. We learned to distinguish between numerical fields, such as house counts, and categorical fields, such as place and tribal names, which needed to be treated as strings.
We also realized that changing the data types alone was not enough. We needed to use an individual point layer rather than relying on aggregated visualizations to display information about each settlement. With guidance from ChatGPT, we adjusted the visualization and were eventually able to display both the place names and their associated information through the map’s tooltips.

<figure>
  <img
    src="{{ '/assets/images/image 6.png' | relative_url }}"
    alt="image 6"
    style="max-width: 100%; height: auto;">

  <figcaption>image 6</figcaption>
</figure>
 
## 4. What the data reveals about Oman

The most interesting part of this project was examining how tribal affiliations and recorded house counts were distributed geographically. Even though our dataset is not a complete representation of historical Oman, several patterns became visible when we considered the records together.

One noticeable pattern is the repeated appearance of certain tribes across multiple settlements. Bani Hina is a good example, appearing in 21 records across several geographical areas, including Hajar, Wādi Samāil, Wādi Fara', Wādi Bani Ghāfir, and Omān Proper. Their recorded house counts also vary considerably, from 20 houses in Hārithīyah to 300 in Nizwa. This could demonstrate that the same tribal affiliation can appear across multiple settlements with different recorded settlement sizes. It also shows why retaining the location of each record was important because grouping all information under one tribal name would have removed the geographical differences between settlements.

<figure>
  <img
    src="{{ '/assets/images/image 2.png' | relative_url }}"
    alt="image 2"
    style="max-width: 100%; height: auto;">

  <figcaption>image 2</figcaption>
</figure>

Another interesting concentration appears around Wādi Dima in Eastern Hajar. The majority of the records in this area are associated with Bani Shahaim. We identified settlements including Dairah, Samūt, Ghamsah, Qaryah, Hail, Qutaifi, Barkyāt, Ahla, Samhān, Hisn, Hārrah, Qabsah, and Auf. Their recorded house counts range from 10 in Qabsah to 180 in Hisn. The repeated association of Bani Shahaim with several nearby settlements makes this one of the clearest geographical patterns in our dataset. At the same time, the variation in house counts shows that settlements within the same area were not necessarily similar in size.

<figure>
  <img
    src="{{ '/assets/images/image 3.png' | relative_url }}"
    alt="image 3"
    style="max-width: 100%; height: auto;">

  <figcaption>image 3</figcaption>
</figure>
 
A similar pattern can be observed in Ruūs-al-Jibāl in Musandam, where several settlements are associated with Dhahūriyīn. These include Film, Habalain, Mansal, Maqāqah, and Qānah, alongside settlements around Khor-ash-Sham and Ghubbat Shābūs. Their recorded house counts range from just 6 in Mansal to 100 in Maqāqah. This provides another example of a tribal name appearing repeatedly across geographically connected settlements, while the recorded number of houses differs between them.

<figure>
  <img
    src="{{ '/assets/images/image 4.png' | relative_url }}"
    alt="image 4"
    style="max-width: 100%; height: auto;">

  <figcaption>image 4</figcaption>
</figure>
 
The records from Dhufār offer a different perspective. Several settlements are associated with Āl Kathīr, including Auqad, Dahārīz, Hāfah, and Rizāt. However, these entries also demonstrate why looking only at house counts would have been limiting. The Gazetteer describes different types of structures, including mud houses, stone and mud houses, huts, and stone buildings. Other entries refer to forts, ruined sites, and deserted settlements. Retaining the Structure column allowed us to preserve these distinctions and recognize that the historical descriptions contain information beyond the number of houses.

We also found that some settlements had records involving multiple tribes. For example, Dhank Town includes 400 houses associated with Na'īm and a separate figure of 300 shared between Na'īm and Shakūr. Other examples include Bidāh and Sā'idah in Dūt and Bani Qitab and Balūchi in Aflāj Bani Qitab. These records show the importance of our Shared_Tribe column. Without it, we could have incorrectly interpreted combined figures as belonging to one tribe.
Looking at the larger house counts, some of the highest recorded figures include 600 at Aflāj Bani Qitab, 400 for the Na'īm entry in Dhank Town, 300 in Nizwa, 300 in Muti, and 280 in Khatwah. These figures provide an opportunity to compare the recorded scale of different settlements. However, we should be careful not to interpret house counts as population figures, since the number of houses does not necessarily indicate how many people lived in a particular location.

The map shows that the records are distributed across several geographical areas  instead of forming one continuous concentration. We can identify groupings around Hajar and Wādi Dima, Dhāhirah and Bātinah, the interior of Oman, Dhufār, and Musandam. Seeing these records geographically makes it easier to recognize relationships between settlements that might not be immediately obvious when reading individual Gazetteer entries.

## 5. Limitations and final reflections

Despite the patterns we identified, our dataset has several limitations. The information depends on what Lorimer’s Gazetteer recorded, and entries do not always provide the same level of detail. Some records have missing house counts, tribal affiliations, subtribal information, or coordinates. Additionally, the coordinates obtained through Zenodo should be understood as geographical references rather than proof of the exact historical location of every settlement.

Using Gemini also required careful verification. Although it made extracting information from numerous screenshots more efficient, we still had to check its output against the original pages, correct the table structure, and decide how to categorize certain records. AI assisted with the process, but the reliability of the final dataset depended on our own decisions and verification.

One of our biggest takeaways was that transforming historical text into spatial data involves interpretation. Decisions about how to structure a table, distinguish between individual and shared tribal counts, categorize settlements, and assign geographical coordinates all influence the final visualization. The original Gazetteer was not designed as a dataset for geographical analysis, so turning it into one required us to make these decisions carefully.

We began with an interest in religion but changed direction when we realized that the available information was not consistent enough for meaningful comparison. By focusing on houses, tribes, and settlements, we were able to create a more structured dataset and explore patterns across different parts of Oman. 

