# Lead-Scoring-Data-Analysis
#### Build a model to assign a lead score to each of the leads such that the customers with higher lead score have a higher conversion chance and the customers with lower lead score have a lower conversion chance.

### Introduction :
An education company named X Education sells online courses to industry professionals. On any given day, many professionals who are interested in the courses land on their website and browse for courses.

The company markets its courses on various websites and search engines such as Google. Once these people access the website, they can browse the courses, fill out a course form, or watch videos. When these people fill out a form providing their email address or phone number, they are classified as leads. In addition, the company also obtains leads through previous referrals. Once these leads are captured, sales team employees start making calls, writing emails, and more.Through this process, some of the leads are converted while most are not. The typical lead conversion rate in X Education is around 30%.

Now, although X Education is getting a lot of leads, it has a very low lead conversion rate. For example, if, say, they acquire 100 leads in a day, only about 30 of them convert. To make this process more efficient, the company wants to identify the most potential leads, also called “Hot Leads”. If they are successful in identifying this set of leads, the lead conversion rate should increase as the sales team will focus more on communicating with potential leads rather than making calls to everyone.

There are many leads produced in the first stage (top), but only a handful of them become paying clients in the second stage (bottom). In order to obtain a better lead conversion, you need to nurture the potential leads properly in the intermediate stage (e.g., educating the leads about the product, communicating frequently, etc.).

X Education wishes to choose the most promising leaders, that is to say leader, who are probably transformed into payment of the clientele. The Company requires you to build a model where you need to assign a note on leaders on each leaders, such as customers with higher main indicator H, have a higher conversion chance and customers with a level of higher foreground evaluation have a lower conversion chance.

### Problem Statement :
 * X Education has appointed you to help them select the most promising leads, i.e. the leads that are most likely to convert into paying customers.
 * The company requires you to build a model wherein you need to assign a lead score to each of the leads such that the customers with higher lead score have a higher conversion chance and the customers with lower lead score have a lower conversion chance.
 * The CEO, in particular, has given a ballpark of the target lead conversion rate to be around 80%.

### Objective:
 * Build a logistic regression model to assign a lead score between 0 and 100 to each of the leads which can be used by the company to target potential leads.
 * A higher score would mean that the lead is hot, i.e. is most likely to convert whereas a lower score would mean that the lead is cold and will mostly not get converted.

### Description of Dataset :
   **1. Prospect ID —** A unique ID with which the customer is identified.

   **2. Lead Number —** A lead number assigned to each lead procured.

   **3. Lead Origin —** The origin identifier with which the customer was identified to be a lead. Includes API, Landing Page Submission, etc.

   **4. Lead Source —** The source of the lead. Includes Google, Organic Search, Olark Chat, etc.

   **5. Do Not Email -** An indicator variable selected by the customer wherein they select whether of not they want to be emailed about the course or not.
   
   **6. Do Not Call —** An indicator variable selected by the customer wherein they select whether of not they want to be called about the course or not.

   **7. Converted —** The target variable. Indicates whether a lead has been successfully converted or not.

   **8. Total Visits —** The total number of visits made by the customer on the website.

   **9. Total Time Spent on Website —** The total time spent by the customer on the website.

   **10. Page Views Per Visit —** Average number of pages on the website viewed during the visits.
   
   **11. Last Activity —** Last activity performed by the customer. Includes Email Opened, Olark Chat Conversation, etc.

   **12. Country —** The country of the customer.

   **13. Specialization —** The industry domain in which the customer worked before. Includes the level ‘Select Specialization’ which means the customer had not selected this option while filling the form.

   **14. How did you hear about X Education —** The source from which the customer heard about X Education.

   **15. What is your current occupation —** Indicates whether the customer is a student, unemployed or employed.
   
   **16. What matters most to you in choosing this course An option selected by the customer —** indicating what is their main motto behind doing this course.

   **17. Search —** Indicating whether the customer had seen the ad in any of the listed items.

   **18. Magazine**

   **19. Newspaper Article**

   **20. X Education Forums**

   **21. Newspaper**

   **22. Digital Advertisement**

   **23. Through Recommendations —** Indicates whether the customer came in through recommendations.

   **24. Receive More Updates About Our Courses —** Indicates whether the customer chose to receive more updates about the courses.

   **25. Tags —** Tags assigned to customers indicating the current status of the lead.

   **26. Lead Quality —** Indicates the quality of lead based on the data and intuition the employee who has been assigned to the lead.

   **27. Update me on Supply Chain Content —** Indicates whether the customer wants updates on the Supply Chain Content.

   **28. Get updates on DM Content —** Indicates whether the customer wants updates on the DM Content.

   **29. Lead Profile —** A lead level assigned to each customer based on their profile.

   **30. City —** The city of the customer.

   **31. Asymmetric Activity Index —** An index and score assigned to each customer based on their activity and their profile

   **32. Asymmetric Profile Index**

   **33. Asymmetric Activity Score**

   **34. Asymmetric Profile Score**

   **35. I agree to pay the amount through cheque —** Indicates whether the customer has agreed to pay the amount through cheque or not.

   **36. a free copy of Mastering The Interview —** Indicates whether the customer wants a free copy of ‘Mastering the Interview’ or not.

   **37. Last Notable Activity —** The last notable activity performed by the student.


### Dataset Source :
https://www.kaggle.com/amritachatterjee09/lead-scoring-dataset


### Exploratory Data Analysis

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/01.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/02.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/03.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/04.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/05.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/06.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/07.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/08.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/09.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/10.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/11.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/12.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/13.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/14.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/15.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/16.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/17.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/18.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/19.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/20.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/21.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/22.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/23.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/24.jpg)

![](https://github.com/ShivankUdayawal/Lead-Scoring-Data-Analysis/blob/main/Data%20Visualization/25.jpg)
