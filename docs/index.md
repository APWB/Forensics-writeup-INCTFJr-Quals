<html>
<head>
<title>Inctfj qualifier writeups some</title>
</head>
<body>
<p>
So, I played <a href="https://app.traboda.com/contest/inctf-jr-21-quals"> Inctf jr qualifiers </a> this winter...was a fun filled contest...It was also my first CTF..XD
Got qualified for the finals though
Posting writeups of some of the forensics challs I solved....
</p>
Forensics challs were really easy..well for me
<h3> Chall name : Dark Wave </h3>
<h4>Category:hard
</h4>
<h5>Description:Can you visualize sound?</h5>
<p>
So we were provided with a audio file
Now, this chall's category was given as hard..but looked the easiest to me
The solve was really simple.
<br>
The description told can u visualise sound?
<br>
So my first guess was Audacity
I opened the audio file given in audacity and opened the sound in spectogram format..and there it's. 
The flag was there only...
</p>
<hr>
<br>
<h3> Chall name:Tweak Me </h3>
<h4> Category: Medium</h4>
<h5> Description :Tweak the Image width by width until it shows what you want it to show! </h5>
<p>
Once again an easy chall..a simple one 
<br>
I just opened the image file provided to us in a hex editor..made the width 1600 and it gave me the flag
</p>
<hr>
<h3> Chall name: Finding Data </h3>
<h4> Category : Medium </h3>
<h5> Description : Sometimes, we see only what we want to see. Look deeper... </h5>
<p>
While reading the description..one word hit me hard
<br>
The word was <strong>deeper</strong>
<br>
My first guess was to use binwalk tool..And it turned out that a zip file was embedded in the image.
I extracted it...Now it needed password
<br>
So I used exiftool and found the password 
<br>
Used it and got the flag
</p>
<hr>
<br>
<h3> Chall name : Corrupt </h3>
<h4> Category: Medium </h4>
<h5> Description : Do you believe in 'magic'? </h5>
<p>
So we were provided with a zip file
Now this word, <strong>magic</strong> striked me...<i>Magic Numbers</i>
So, I opened the file in a hex editor..as predicted the file header was wrong
<br>
Corrected it and got the flag
</p>
<hr>
<br>
<h3> Chall Name: White House </h3>
<h4> Category : Easy </h4>
<h5> Description : Can you retrieve the secret message?
<br>
Key:"am9obiBjZW5hCg=="
<br>
This key will help you on some stage :) </h5>
<p>
Well, this was easy.We were given a text file..I decoded the key given in base64 format in the description Used the key with <i>Stegsnow</i> and got the flag
</p>
<hr>
<br>
<h3>VIBGYOR</h3>
<h4>Category:Easy</h4>
<h5> Description : Alike Every rainbow that shines in the sky consists of seven colors. Every pixel that shines in the image consists of certain colours. </h5>
<p>
Just open the image file provided in stegsolve ...change the colors until u get the flag 
</p>
<hr>
<br>
<h3> Chall Name : Track Me </h3>
<h4>category : Easy </h4>
<h5> Description : It's easy to identify specific crimes and follow them up. </h5>
<p>
Open the packet capture provided in wireshark, analyse, in one of the packets, the flag is there 
</p>
<hr>
<br>
<h3> Chall name : End of It </h3>
<h4> Category : easy </h4>
<h5> Description : Sometimes you will get what you need only at the end. </h5>
<p>
I was the first one to solve this chall
<br>
Open the image provided in a hex editor..after the EOF, the flag is given 
</p>
<hr>
<br>
<h3> Easy-Peasy </h3>
<h4> Category : easy </h4>
<h5> Description : Try to reveal what is hidden in this jpg. </h5>
<p>
This chall was really easy.
Use jsteg 
<i>jsteg reveal <filename></i>
And this gave the flag
</p>
<hr>
<br>
<h3> All the glitters is not gold </h3>
<h4>Category:Easy</h4>
<h5> Description : Shakespeare gave three Poems to his three children respectively and asked them to complete it by finding the missing words. Can you help them to complete it?
<br>
If the link doesn't open, try with VPN!
<br>
Flag format : inctfj{ruby_gold_silver} (Use lowercase letters and concatenate the words)</h5>
<p>
There was a qr code image we were provided with
<br>
Using <i>Barimg</i> tool, I scanned the qr code..It gave a link..there were three text files there..all with one balnkspace as the description told
<br>
So, Shakespeare was a poet, right?
<br>
So these must be lines of his poem..Yess. That is it..Searched the lines in google..got the words to be filled.. done!
<p>
<hr>
<hr>
Well, hope u liked and understood my writeup
</body>
</body>
</html>
