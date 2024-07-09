# Challenge Description:

<div align="justify">
> Identify any social-media accounts or websites used by the person-of-interest <br>
> Build up a profile of the person-of-interest<br>
> Find any evidence of malicious behaviour<br><br>

  You work for a law enforcement organisation, and you have been assigned to track a person-of-interest, that is believed to be associated with a hacking group that recently compromised a 
  Managed Service Provider (MSP) and are trying to sell the stolen credentials on both the clear net and dark web. Another team is focusing on the dark web lead, so you have been tasked with 
  using OSINT sources to build up a profile on the individual and attempt to locate any evidence that links them to the MSP breach and sale of account details. You have been provided with some information 
  to start your investigation. You should use any of the sources or tools taught in this course, that you deem to be applicable and appropriate. 
  We know that the email address used to register the Twitter account is fake, so do not include this in your report.
</div>

## Your manager has provided you with the following starting information:

Twitter handle used by actor: @sp1ritfyre

## Questions:
Investigation into MSP data breach. Clear web investigation team.

Known Info:

Twitter Handle: @sp1ritfyre

Required Info: <br>
First Name: <br>
Last Name: <br>
Age: <br>
Country: <br>
Interests (5 minimum): <br>
Hacker's employer (company name): <br>
Hacker's position within company: <br>
Self-Owned Website (Hacker owns the domain): <br>
Other Websites (Person does not own the domain, such as blogs): <br>
Any URLs of webpages that directly tie individual to MSP breach: <br>
What email addresses have been used by the hacker? 

## Answers:
1. What is the hacker's first name? Sam <br>
2. What is the hacker's last name? Woods <br>
3. What is the hacker's age? 23 <br>
4. What country does the hacker live in? United Kingdom <br>
5. What are some of the hacker's interests? Security, Photography, Gaming, Malware Analysis and Camping <br>
6. What company does the hacker work for? Philman Security Inc <br>
7. What is the hacker's position within the company? Junior Penetration Tester <br>
8. What is the full url of the website owned by the hacker? https://redhunt.net <br>
9. List any full URLs of websites not owned, but used by the hacker (Blogs only) https://sp1ritfyrehackerstories.blogspot.com/ https://sammiewoodsec.blogspot.com/ <br>
10. What email address has been used by the hacker? d1ved33p@gmail.com <br>


## My Investigation:
My only information about the hacker is their Twitter username, so I search for it on Twitter and find their profile. After stalking this person's Twitter, I notice a link in their bio that appears to be a Base64-encoded string.

<div align= "center">
  <img src="https://github.com/Gepzuu/BTJA-Course-Capstone/assets/92858147/a0f5a6a6-6e92-44ee-a96c-23df17f3c7cc" alt="c1">
</div><br>
I check the link to see what it is, but it results in a page error. <br><br>
<div align= "center">
  <img src="https://github.com/Gepzuu/BTJA-Course-Capstone/assets/92858147/ac00c24f-ad4e-44ea-a24a-b1b74ab77818">
</div><br>
I go to Google and search for the username '@sp1ritfyre' and I see a Blogger link with this person username, so I visit it. <br><br>
<div align= "center">
  <img src="https://github.com/Gepzuu/BTJA-Course-Capstone/assets/92858147/be2aabdf-f5ed-471e-bb7f-bf637a924dc5">
</div><br>
I see information about the email and location, but the location is showing random letters and numbers, so I decide to check the email first. I go to inspect the email tag to see what the email is, and it's still too early to tell, but the email is 'd1ved33p@gmail.com'. <br><br>
<div align= "center">
  <img src="https://github.com/Gepzuu/BTJA-Course-Capstone/assets/92858147/da52c304-edef-4741-a470-74c60d62f66d">
</div><br>
After inspecting the email, I return to the main page of the blog to investigate the location that appears to contain random numbers and letters. I go to Google and search for a 'hexadecimal decoder' to decode the location. <br><br>
<div align= "center">
  <img src="https://github.com/Gepzuu/BTJA-Course-Capstone/assets/92858147/ec2ed3af-10ba-42db-b075-e313c7757d4f">
</div><br>
The result is a Blogspot link, which I copy and paste into Google. This takes me to the blog page. <br><br>
<div align= "center">
  <img src="https://github.com/Gepzuu/BTJA-Course-Capstone/assets/92858147/b65783ed-3759-455d-ab93-4e0688671a15">
</div><br>
After checking all the Blogger links, I now have the information I need to answer all the questions. <br><br>
<div align= "center">
  <img src="https://github.com/Gepzuu/BTJA-Course-Capstone/assets/92858147/7d6390cc-dd72-4532-96b3-929a1b40b611">
  <img src="https://github.com/Gepzuu/BTJA-Course-Capstone/assets/92858147/003d77d3-9773-4a30-a28c-4c5f2c7c6519">
  <img src="https://github.com/Gepzuu/BTJA-Course-Capstone/assets/92858147/410ebafb-1b2b-41da-be6f-f91e04b5b27f">
</div><br>



## NOTE:
<div align="center">
This is for educational purposes only <br>
This is a fictional scenario. Any affiliation between the scenario individual and any real person is strictly coincidental.
</div>
   

## Course Link:
<div align="center">
https://www.securityblue.team/courses/open-source-intelligence-training-beginner/
</div>



   





