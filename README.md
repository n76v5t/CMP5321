java cCoursework Assignment Brief
Assessment - Undergraduate

Academic Year 2024-25

Module Title:	Programming for Network Engineers
Module Code:	CMP5321
Assessment Title:	Understanding Automation Concepts
Re-assessment hand in deadline date:	
Return of Feedback date and format	
Support available for students required to submit a re-assessment:	Timetabled support sessions will be arranged for the period immediately preceding the hand-in date
NOTE:	At the first assessment attempt, the full range of marks is available. At the re-assessment attempt the mark is capped and the maximum mark that can be achieved is 40%.
Assessment Summary	

IMPORTANT STATEMENTS

Undergraduate Regulations

For courses accredited by professional bodies such as the IET (Institution of Engineering and Technology) there are some exemptions from the standard regulations and these are detailed in your Programme Handbook

Cheating and Plagiarism

Both cheating and plagiarism are totally unacceptable and the University maintains a strict policy against them.  It is YOUR responsibility to be aware of this policy and to act accordingly. Please refer to the Academic Registry Guidance at https://icity.bcu.ac.uk/Academic-Registry/Information-for-Students/Assessment/Avoiding-Allegations-of-Cheating

The basic principles are:
Don’t pass off anyone else’s work as your own, including work from “essay banks”. This is plagiarism and is viewed extremely seriously by the University.
Don’t submit a piece of work in whole or in part that has already been submitted for assessment elsewhere. This is called duplication and, like plagiarism, is viewed extremely seriously by the University.
Always acknowledge all of the sources that you have used in your coursework assignment or project.
If you are using the exact words of another person, always put them in quotation marks.
Check that you know whether the coursework is to be produced individually or whether you can work with others.
If you are doing group work, be sure about what you are supposed to do on your own.
Never make up or falsify data to prove your point.
Never allow others to copy your work.
Never lend disks, memory sticks or copies of your coursework to any other student in the University; this may lead you being accused of collusion.

By submitting coursework, either physically or electronically, you are confirming that it is your own work (or, in the case of a group submission, that it is the result of joint work undertaken by members of the group that you represent) and that you have read and understand the University’s guidance on plagiarism and cheating.

You should be aware that coursework may be submitted to an electronic detection system in order to help ascertain if any plagiarised material is present. You may check your own work prior to submission using Turnitin at the Formative Moodle Site.  If you have queries about what constitutes plagiarism, please speak to your module tutor or the Centre for Academic Success.

Electronic Submission of Work

It is your responsibility to ensure that work submitted in electronic format can be opened on a faculty computer and to check that any electronic submissions have been successfully uploaded. If it cannot be opened it will not be marked. Any required file formats will be specified i代 写CMP5321、Python
代做程序编程语言n the assignment brief and failure to comply with these submission requirements will result in work not being marked.  You must retain a copy of all electronic work you have submitted and re-submit if requested.

Assessment Details: 

Title: Network Automation Principles and Practice

Type: Coursework 

Style: Report

For this coursework, you are tasked with simulating a real-world network design and automation task to understand the practical applications of Python in networking. These exercises will promo teamwork, problem-solving, and application of programming concepts.

Assessment Part 1 (30%): 
Group Coursework (form into groups of up to 4 students.)
Your group have been tasked by an external company to improve their network infrastructure by proposing a new network design. They are expanding their operations so need to embrace a more efficient, scalable, and automated network.
Pick one of the following departments:
a.Sales Department:  Design a topology and IP scheme for the sales department, consisting of 20 PCs spread across two floors.
b.HR Department: Design a topology and IP scheme for the HR department, consisting of 15 PC across one floor.
c.IT Department: Design a topology and IP scheme for the IT departments 10 PCs – they require to separate IP schemes (one for developers and one for network engineers)
Tasks:
a.Design the topology and address scheme for your chosen department, making sure it meets the structural requirements – you do not need to consider VLANs etc.! Provide a short description with your rationale.
b.Write a short Python script to generate the addresses for your proposed scheme, and output the percentage usage of the address range.
Example topology:

Figure 1 Example topology

Example address scheme:
Network Address	Netmask
192.168.1.0	255.255.255.0 /24 (256 addresses)
Assignment:
Router/Gateway	192.168.1.1
Network printers	192.168.1.10-19
PCs	192.168.1.20-40
Example script:
def generate_ips(base, start, end):
	return [base +str(i) for i in range(start, end+1)]
ip_list = generate_ips(“192.168.1.”, 10, 20)
for ip in ip_list:
	print(ip)
Example script with error handling:
def generate_ips(base, start, end):
    try:
        if not (1 <= start < end <= 254):
            raise ValueError("Start must be less than End, must be in the range of 1-254.")        
        return [base + str(i) for i in range(start, end+1)]
        
    except ValueError as e:
        print(f"Input error: {e}")
    except Exception as e:
        print(f"An unexpected error occurred: {e}")

ip_list = generate_ips("192.168.1.", 10, 20)

if ip_list:
    for ip in ip_list:
        print(ip)

Produce a document containing the work you have produced above, make sure your document contains:
1.Your group members names
2.The network topology
3.The addressing scheme (example tables shown above)
4.The script to generate the addresses based on your scheme
5.Design documentation:
a.Topology design choice(s)
b.IP/Netmask design rationale
c.Security measures
d.Python script explanation
Additional information: 

For advice on writing style, referencing and academic skills, please make use of the Centre for Academic Success: 

         
加QQ：99515681  WX：codinghelp
