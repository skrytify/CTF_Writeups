
` 
Here we land in this page.
![Img 1](https://github.com/skrytify/CTF_Writeups/blob/sub/HTB_LoveTok_Writeups./Images/Screenshot%202023-09-04%20195749.png)

When we click on the red area URL changed to something else.


 ![Img 2](https://github.com/skrytify/CTF_Writeups/blob/sub/HTB_LoveTok_Writeups./Images/Screenshot%202023-09-04%20195826.png)

 
So I tried something else like “test”.


![](https://github.com/skrytify/CTF_Writeups/blob/sub/HTB_LoveTok_Writeups./Images/Screenshot%202023-09-04%20195910.png)
Here we can see it has displayed something new. Then I started thinking what can I do.
After a time, I thought of getting web shell. 
Parameter: ${system($_GET[cmd])}&cmd=ls
And we got it.
 ![](https://github.com/skrytify/CTF_Writeups/blob/sub/HTB_LoveTok_Writeups./Images/Screenshot%202023-09-04%20200326.png)
Here are the same files that we had downloaded earlier. 
So I tried getting back on the directory. Using “ls ../”
 ![](https://github.com/skrytify/CTF_Writeups/blob/sub/HTB_LoveTok_Writeups./Images/Screenshot%202023-09-04%20200552.png)
Here we can find a file name flag so let’s read it using cat.
: cmd=cat ../ flagyE9AQ
`
