<p align="center">
<img src="https://imgur.com/OOeFFhB.png"/>
<h1> Splunk Walk-Through </h1>

This walkthrough demonstrates a few basic commands that can be used in Splunk to manipulate logs and data. Specifically, we will be issuing commands from Splunk's Search Processing Language (SPL) which is able to search for, filter, modify, and manipulate log data.
.<br />


<h2>Environments and Technologies Used</h2>

- Windows 10 Desktop
- Splunk Enterprise

<h2>Operating Systems Used </h2>

- Windows 10</b> 


<p>Overview</p>

<p>
<img src = "https://imgur.com/Xd2j7bu.png" " height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
 <p>
1. Stats: The stats command is used to perform a certain action on the search results. This includes calculating the sum, average, minimum, and maximum of values.

</p>                                                                                                    
                                                                                                     
<p>
<img src= "https://imgur.com/KMAgT05.png" " height="80%" width="80%" alt="Disk Sanitization Steps" />
</p>                                                                                            
                                                                                                 
2.  Eval: The eval command allows users to create new fields or edit fields.                                                                   
</p>
<br />

<p>
<img src="https://imgur.com/c6RJVWL.png" />
</p>

<p>
3. Strptime: The strptime command is used to convert a human-readable time to a Unix-based time. To strptime command comes in the form of two arguments. The first string of the argument describes the data and time and the second argument describes how the data and time is structured in the string.
</p>
<br />
