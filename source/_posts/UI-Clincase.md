---
title: Enhance ePRO’s electronics diary entry user experience
date: 2019-07-27 20:11:04
categories: portfolio
tags:
  - portfolio
cover_image: /images/ePro.png
---

<p style="color:#aaa;">Clincase | Year: 2017-2019</p>


### Overview
When I worked as part-time UX engineer in Clincase, I was in the team which responsible for ePRO product. ePRO, so called electronic Patient-Reported Outcome, is mainly used in clinical trials for patients to complete the questionnaires and report their outcomes by electronic methods without subjecting to their hospital visits.

One of the important requirement for ePRO is letting patients to complete their data entry within certain time period. Data records should be taken at the specified time to prevent forward filling and should be completed before the specified time to prohibit backfilling. Technically, it’s definitely doable, but our mission is to help patients better fulfilling this through UI/UX enhancement.

### User Research and Problem Statement
To start off, we conducted a user research by interviewing one of the manager in CRO (Clinical Research Organization) – KCR. KCR is actually our client in this case who request us to build ePRO. Although ePRO's end users would be patients, but due to privacy concerns, we were unable to get in touch with patients. Fortunately, the KCR manager fully grasped the patient's condition based on her experienced observation and provided a relatively clear and detailed description of the patient's pain points.

Here are the main pain points we found out from the interview:
> Pain point #1: Patients often forgot when shall they enter their data even though they have been told several times before by doctor.
> Pain point #2: Patients often failed to complete their data entries, causing those data can’t be used for study.

### Persona and Insight
> Users(patients) need a way to inform themselves when and how many entries they need to enter and stay concentrated while doing it.

After the interview, I first created a provisional persona to help myself better imagine the ePRO usage scenario. This persona was something that I came back to throughout the project to guide my design decisions and priorities.
<div style="text-align:center;margin-bottom:40px;">
<img src="https://drive.google.com/uc?export=view&id=1cNrKcX5kzka8YWUqVM7WB2_Q02v1FjnQ" width="100%" height="auto" />
</div>


### Ideate and Prototype
There are two features we decided to focus on ideating in order to achieve our insight: **calendar** (for showing when and how many entries) and **questionnaire entry flow** (for helping users to stay concentrated while doing it).

**Calendar Lo-fi Mockup:** We thought it's important to add the calendar feature to ePRO to help users track and arrange their schedule.
<div style="display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;margin-bottom:10px;">
<img src="https://drive.google.com/uc?export=view&id=1R8OI-r1s6Wr69Ax7dnhi5xBFT3x6Uzag" width="213px" height="auto"/>
<img src="https://drive.google.com/uc?export=view&id=1Rji9NcrHWA8HM15ejIWezsTM7DDmDOEM" width="213px" height="auto"/>
<img src="https://drive.google.com/uc?export=view&id=1A9WO0Jq6tKIDCMhXSZk8CLnsgvUPh3fp" width="213px" height="auto"/>
</div>
**Calendar Med-fi Mockup:** Besides only showing calendar, we also added todo entries to each day with time notification, so that users know when and how many entries they need to enter.
<div style="display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;margin-bottom:40px;">
<img src="https://drive.google.com/uc?export=view&id=14EXxo6rkelrbanpmPPjVNAKGOM6V_I7J" width="213px" height="auto"/>
<img src="https://drive.google.com/uc?export=view&id=1pCbi6DbnyH-amwpRk0NYzZDiVP6gtoh-" width="213px" height="auto"/>
<img src="https://drive.google.com/uc?export=view&id=1p5ayVo_3Q6hkVvES5DkZGyvbAFsNVxo2" width="213px" height="auto"/>
</div>

---

**Questionnaire Lo-fi Mockup:** To help users stay concentrated in the flow, we aimed to make each entry screen clean by showing only one question per screen.

<div style="display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;margin-bottom:40px;">
<img src="https://drive.google.com/uc?export=view&id=1K_7Z9pW1aO_pUlRvMO_AVrllmO4xubUz" width="213px" height="auto"/>
<img src="https://drive.google.com/uc?export=view&id=1apSkMrG6pJjY-xJTvPIH50_ScEbwgqZy" width="213px" height="auto"/>
<img src="https://drive.google.com/uc?export=view&id=1Yg4De38c2wDSyxfcwyIH4ypfSm7-2XE5" width="213px" height="auto"/>
</div>

**Questionnaire Med-fi Mockup:** Animations were experimented on questionnaire to smoothen the transition of questions. I assumed providing smooth animations can create delightful data entry experience and further help users concentrated in the flow.

<div style="display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;margin-bottom:10px;">
<img src="https://drive.google.com/uc?export=view&id=1esNYELYwRA9VosrSSG27K0HtL2GYSsyh" width="213px" height="auto"/>
<img src="https://drive.google.com/uc?export=view&id=1ehlNkNOwmE-jgNGbX9GsgCyGR2jH4Gq6" width="213px" height="auto"/>
<img src="https://drive.google.com/uc?export=view&id=1NVnkkXgVCaYKzujQxw7fIOk8imoQNaZ2" width="213px" height="auto"/>
</div>
<div style="text-align:center;margin-bottom:40px;">
<video id="video"  preload="auto" autoplay loop>
<source id="mp4" src="/images/Proquestion.mp4" type="video/mp4">
</video>
</div>

### Test and Refine
We did several internal tests by uploading our Med-fi mockups to InVision and let people in KCR to test them out. They provided us some feedbacks, especially on the calendar feature.  

**Calendar:**
As mentioned before, it's really important that patients enter data at the right time period, forbidding forward and back filling.
<div style="display:flex;align-items:center;justify-content:space-between;margin-bottom:10px;">
<img src="https://drive.google.com/uc?export=view&id=1LXkblDUkn23WHufDzaKupJ6JGsqz-3Rx" width="200px" height="auto"/>
<div style="margin-left: 20px">The Med-fi calendar mockup shows "when" shall the entry be taken, ex: morning or during night.<br />But this doesn't show urgency to users. For example, in the morning, users probably know they need to enter their data during night, yet lots of things happened during the day and they are likely to forget their data entry if no one continue to remind them.</div>
</div>

We redesigned the calendar page by changing the text ”morning/during night” to “certain time left”. Start counting down when that entry were open to enter. Colors were also applied to indicate urgency ( blue for > 1 hr, amber for within 1 hr, red for < 1 hr ). On the other hand, we added push notification feature to remind users every hour.

<div style="display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;margin-bottom:10px;">
<img src="https://drive.google.com/uc?export=view&id=1b3uIBUQQPzGSAb07lX5qUsV6n6Qt8Otd" width="213px" height="auto"/>
<img src="https://drive.google.com/uc?export=view&id=1SAC90_Pfi_brTWb1ddmiiWYg7L5A2Cg-" width="213px" height="auto"/>
<img src="https://drive.google.com/uc?export=view&id=1bhzcjFSQwCScs1v2H9XcCjs9RZ2EvkMt" width="213px" height="auto"/>
</div>

### Final Design and Takeaways
<div style="text-align:center;margin-bottom:40px;">
<img src="https://drive.google.com/uc?export=view&id=1UjZ4GYRQZlL1-wA5-8CFh7-pH5As15Zp" width="100%" height="auto" />
</div>
<div style="text-align:center;margin-bottom:40px;">
<img src="https://drive.google.com/uc?export=view&id=1OTc3LphW7JQ9t5k9cqUOJPRcbQzyy3UI" width="100%" height="auto" />
</div>

ePRO is a powerful tool for patients to complete their data entries for clinical trial from anywhere without subjecting to their hospital visits. Ensuring patients complete data entries within specified time is one of the biggest requirements and challenges. But patients are human too, human often forget things and lose patience with tedious questionnaire. So it's important to remind users rather than hoping them to remember by themselves and make the data entry flow friction-less as possible. Sometimes a change as small as adding animations or changing texts can make a difference.
