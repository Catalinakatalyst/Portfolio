# Phishing Simulation Project with GoPhish

## Project Overview  
This project demonstrates how to set up and run a phishing simulation campaign using GoPhish to raise awareness about phishing risks and improve user vigilance.

## Tools Used  
- [GoPhish](https://getgophish.com/) – Open-source phishing framework  
- Kali Linux to host and run GoPhish  
- Target email accounts (test users or other personal accounts)

## Setup Steps

1. **Download and Install GoPhish**  
   - Download the latest GoPhish release from [GitHub](https://github.com/gophish/gophish/releases)  
   - Unzip the file and go to the gophish dir
     cd gophish-V0.12.1-linux-64bit
   - Run gophish
     sudo gophish
     

2. **Access GoPhish Web UI**  
   - Open browser at https://127.0.0.1:3333 (This is the localhost IP) 
   - Login with default credentials (`admin` / `gophish`) ** this would be reset immediately the default password is added **

3. **Create Email Template**  
   - Template
     Envelope address - ITTeams@onmicros0ft.com

     Subject: Reminder: Reset Password Soon!
     Body:
     Hi there,

     Your password would be expiring in 3 days, use the link below to reset the password.

     https://catalinatech.onmicros0ft.com/resetpassword/
     
     Password requirements
     Must be 16 characters long
     Must have an uppercase letter, lowercase letter, digits and special characters (!@£$%&*(),.?)

     Technical Support Team
     Catalina Technologies

     
   - In my case I used a reset your password template with an embedded microsoft login page URL 
  
       
5. **Create Landing Page**  
   - Clone a legitimate login page I cloned the microsoft login page - https://login.microsoftonline.com/
   - Configure it in GoPhish as the destination for your phishing email

6. **Create and Launch Campaign**  
   - Add your target email addresses (emails used belong to me)
   - Schedule and send the phishing emails  
   - Monitor campaign progress through the GoPhish dashboard

## Awareness & Reporting

- Track open, click, and submission rates of the campaign  
- Identify users who engaged with the phishing simulation  
- Provide targeted training or communication to improve awareness  
- Create a simple one-page report summarizing campaign results and lessons learned

## Key Takeaways

- Regular phishing simulations help users recognize suspicious emails  
- Awareness training reduces risk of real phishing attacks  
- Monitoring and reporting provide actionable insights for security teams

---

*This project showcases practical phishing simulation and user awareness skills, valuable for strengthening organizational security posture.*
