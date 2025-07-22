## Introduction 
Welcome to my Nessus project - In this project, I'll be using Nessus to conduct a vulnerability scan of Metasploitable 2. 
Metaploitable2 is a free to use cybersecurity product from Rapid7.
It is a Debian based linux distribution which is deliberately designed to include weaknesses and exploits for cybersecurity training. 
Below I will show the steps of the process of how I did this. 

## Step 1. 

I first started by installing Nessus on Kali Linux. 

![Nessus-project 1 ](https://github.com/JWALL000/Nessus/blob/main/Step%201%20-%20welcome%20to%20my%20nessus%20project%20-%20installing%20on%20Kali%20linux.PNG)

## Step 2. 

After this, Nessus started unpacking. 

![Nessus-project 2 ](https://github.com/JWALL000/Nessus/blob/main/Step%202%20-%20unpacking%20Nessus.PNG)

## Step 3. 

Next, I opened the web UI for Nessus, It was time to make a Tenable account for Nessus. In this Project I used Nessus Essentials as it was the free version offered by Tenable and included everything we needed to start doing scans. 

![Nessus-project 3 ](https://github.com/JWALL000/Nessus/blob/main/Step%203%20-%20Opening%20the%20web%20UI%20with%20the%20ip%20of%20local%20host.PNG)

## Step 4. 

Next, I had to wait for Nessus to finish initializing - This step required some patience as it took a while for Nessus to get fully set up. 

![Nessus-project 4 ](https://github.com/JWALL000/Nessus/blob/main/Step%204%20-%20After%20creating%20my%20account%20-%20I%20had%20to%20wait%20for%20Nessus%20to%20finish%20intializing.PNG)

## Step 5. 

After all the plugins for Nessus were finished installing, we were ready to start scanning. 

![Nessus-project 5 ](https://github.com/JWALL000/Nessus/blob/main/Step%205%20-%20After%20plugins%20were%20finished%20installing.PNG)

## Step 6. 

I then started with a test scan of my Kali Linux machine to see what results I got. 


![Nessus-project 6 ](https://github.com/JWALL000/Nessus/blob/main/Step%206%20-%20Scanning%20local%20host.PNG)

## Step 7. 

I then waited for Nessus to finish scanning. 

![Nessus-project 7 ](https://github.com/JWALL000/Nessus/blob/main/Step%207%20-%20Vulnerabilities%20show%20up.PNG)

Now we can see our results. But I came to find out later on that this was indeed not a full scan - I fixed this issue later but It gave me an idea of how Nessus scans were carried out. 

![Nessus-project 8 ](https://github.com/JWALL000/Nessus/blob/main/Step%208%20-%20Scan%20still%20running%20-%20finding%20more%20severe%20vulnerabilites%20and%20giving%20them%20a%20CVSS%20score.PNG)

## Step 8 

Now it was time to get Metapsloitable 2 up and running - I headed over to Rapid7s website to download my instance of Metapsloitable 2. 

After that I extracted the files and spun it up in VirtualBox. 

![Nessus-project 9 ](https://github.com/JWALL000/Nessus/blob/main/Step%209%20-%20Getting%20metasploitable%202.PNG)


## Step 9. 

I then started to conduct the scan on Metaploitable but I noticed an issue - I didn't get back the results I expected. This was because I my network settings were incorrect. 

I thought that if I enabled port forwarding on my Metasploitable 2 instance, I would be able to conduct an authorized ssh scan using Nessus. However, this was not the correct way to conduct a full in depth scan. 

After changing my Network settings in both my VMs for Nessus and Metasploitable 2 - I then restarted both machines and got the new IP address for Metasploitable 2. 
The IP below states it is 10.0.2.15 - but after I changed my network settings to host-only network - I had the new correct IP address. 

![Nessus-project 10](https://github.com/JWALL000/Nessus/blob/main/Step%2010%20-%20Scanning%20Metasploitable%202.PNG)


## Step 10. 

Here we can see the results of our scan and as expected, It was full of dangerous vulnerabilities with high CVSS scores. 

![Nessus-project 11](https://github.com/JWALL000/Nessus/blob/main/Step%2011%20-%20Results%20of%20scan.PNG)

## Step 11. 

In this step I exported my findings in the format of a report - this step gave me insight on how vulnerability reports can be structured in life. You can see below all of the vulnerabilites found and in the actual report it was many pages long! 

![Nessus-project 12](https://github.com/JWALL000/Nessus/blob/main/Step%2012%20-%20Report%201.PNG)


## Conclusion 

I thoroughly enjoyed this project and learning about the technologies I used. It was very insightful for me to see how vulnerability scans are conducted and how CVSS scores are generated - I also liked the feature 
built in to Nessus that allows you to export your findings in a report format which I imagine is very useful in real-world scenarios where you have to present your findings to clients. 

Thank you for viewing my Project, hopefully this can provide some insights on how Nessus can be used to conduct vulnerability scans if you weren't familiar already - 

Joseph W. 


























