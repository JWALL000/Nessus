## Introduction 
Welcome to my Nessus project - In this project, Ill be usinig Nessus to conduct a vulnerability scan of Metaploitable 2. 
Metaploitable2 is a free to use cybersecurity product from Rapid7.
It is a debian based linux distrobustion which is deliberatley desgined to include weaknesses and exploits for cybersecurity training. 
Below I will show the steps of the process of how I did this. 

## Step 1. 

I first started by installing Nessus on Kali Linux. 

![Nessus-project 1 ](https://github.com/JWALL000/Nessus/blob/main/Step%201%20-%20welcome%20to%20my%20nessus%20project%20-%20installing%20on%20Kali%20linux.PNG)

## Step 2. 

After this, Nessus started unpacking. 

![Nessus-project 2 ](https://github.com/JWALL000/Nessus/blob/main/Step%202%20-%20unpacking%20Nessus.PNG)

## Step 3. 

Next, I then open the web UI for Nesus, It was time to make a Tennable account for Nessus. In this Project I used Nessus essentials as it was the free version offered by Tennable and included everything we needed to start doing scans. 

![Nessus-project 3 ](https://github.com/JWALL000/Nessus/blob/main/Step%203%20-%20Opening%20the%20web%20UI%20with%20the%20ip%20of%20local%20host.PNG)

## Step 4. 

Next, I had to wait for Nessus to finish intializing - This steo required some patience as it took a while for Nessus to get fully set up. 

![Nessus-project 4 ](https://github.com/JWALL000/Nessus/blob/main/Step%204%20-%20After%20creating%20my%20account%20-%20I%20had%20to%20wait%20for%20Nessus%20to%20finish%20intializing.PNG)

## Step 5. 

After all the plugins for Nessus were finished installing, we were ready to start scanning. 

![Nessus-project 5 ](https://github.com/JWALL000/Nessus/blob/main/Step%205%20-%20After%20plugins%20were%20finished%20installing.PNG)

## Step 6. 

I then started with a test scan of my Kali linux machine to see what results I got. 


![Nessus-project 6 ](https://github.com/JWALL000/Nessus/blob/main/Step%206%20-%20Scanning%20local%20host.PNG)

## Step 7. 

I then waited for Nesuss to finish scanning. 

![Nessus-project 7 ](https://github.com/JWALL000/Nessus/blob/main/Step%207%20-%20Vulnerabilities%20show%20up.PNG)

Now we can see our results. But I came to find out later on that this was indeed not a full scan - I fixed this issue later but It gave me an idea of how Nessus scans were carried out. 

![Nessus-project 8 ](https://github.com/JWALL000/Nessus/blob/main/Step%208%20-%20Scan%20still%20running%20-%20finding%20more%20severe%20vulnerabilites%20and%20giving%20them%20a%20CVSS%20score.PNG)

## Step 8 

Now it was time to get Metaploitable 2 up and running - I headed over to Rapid7s website to download my instance of Metaploitable2. 

After that I extracted the files and span it up in VirtualBox. 

![Nessus-project 9 ](https://github.com/JWALL000/Nessus/blob/main/Step%209%20-%20Getting%20metasploitable%202.PNG)


## Step 9. 

I then started to conduct the scan on Metaploitable but I noticed an issue - I didn't get back the results I expected. This was because I my network settings in my hypervisor were configured incorrectly. 

I thought that If I enabled port forwarding on my Metapoitable2 instance, I would be able to conduct an authorized ssh scan using Nessus. However, this was 
























