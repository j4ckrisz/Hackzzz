---
description: These are notes from Social Engineering by Christopher Hadnagy
---

# Social Engineering by Cristopher hadnagy

## Intro

* SE takes advantage of the fact that gender bias, racial bias, age bias, and status bias (as well as combinations of those biases) exist.
* For instance, imagine you have to infiltrate a client ’ s building. To do so, you need to develop a pretext that allows you to gain entry easily.
* Social engineering is any act that influences a person to take an action that may or may not be in his or her best interests.

## SE Attacks

* **SMiShing**: Yes, this is a real thing, and it stands for SMS phishing, or phishing through text messages.
* **Vishing**: As I already mentioned, this is voice phishing. This has increased as a vector drastically since 2016. It is easy, cheap, and very profi table for the attacker. It is also nearly impossible to locate and then catch the attacker with spoofed numbers calling from outside the country.
* **Phishing** : Th e most talked about topic in the world of social engineering is phishing. In fact, the technical editor on this book, Michele, and I wrote about it in a book titled Phishing Dark Waters: Th e Off ensive and Defensive Sides of Malicious Emails (Wiley, 2016) . (Yes, I did just shamelessly plug one of my other books.) Phishing has been used to shut down manufacturing plants, hack the DNC, breach the White House as well as dozens of major corporations, and steal countless millions of dollars in diff erent scams. Phishing is by far the most dangerous of the four main vectors
* **Impersonate**: I know, we should put some form of ’ishing on this one too, but the best I could do is list it last because it ’ s different. However, its placement in this list by no means indicates that we don ’ t have to worry about it as much as the others. In the past 12 months, we have collected hundreds of stories of people impersonating police, federal agents, and fellow employees committing some truly horrifi c crimes. In April 2017, there was a story of a man who was impersonating the police and was caught. He was dealing in child pornography and using his impersonation to profi t

## The SE Pyramid

### OSINT

OSINT, or Open Source Intelligence, is the life blood of every social engineering engagement. It is also the piece that should have the most time spent on it. Due to that, it occupies the fi rst and largest piece of the pyramid. One piece of this part of the pyramid is rarely addressed: documentation. How will you document, save, and catalog all the information you fi nd? I discuss this key factor a bit more in the next chapter.

### Pretext Development

Based on all the findings from the OSINT period, the next logical step is to start to develop your pretexts. Th is is a crucial piece that ’ s best done with OSINT in mind. During this phase, you see what changes or additions need to be made to ensure success. Th is is also when it becomes clear what props and/or tools are needed.

### Attack Plan

Having a pretext in hand does not mean you are ready. Th e next stage is to plan out the three W ’ s: **what, when, and who**.

» What is the plan? What is it we are going for and trying to achieve? What does the client want? These questions will help develop the next piece.

» When is the best time to launch the attack?

» Who needs to be available at a moment ’ s notice for support or assistance?

### Attack Launch

Now comes the fun part: launching the attacks. With the preparation done on the attack plan, you are prepared to go full steam ahead. It is important to be prepared but not to be so scripted that you can ’ t be dynamic. I am all for having a written plan, and I think it can save you a ton of headaches down the road. Th e caution I have is that if you script out every word or action you feel needs to be taken, you can run into problems when the unexpected happens. Your brain realizes there is nothing on the script to help, and you begin to stutter, get nervous, and show signs of fear. Th is can really ruin your ability to succeed. Instead of scripting, I suggest using an outline, which gives you a path to follow but allows for artistic freedom.

### Reporting

Wait—don ’ t skip over this section. Come back and read it. Yes, reporting is not fun, but you can think of it this way: Your customer just paid you x dollars to perform some services, and most likely, you were pretty darn successful in those attacks.

Example:

1. The attackers investigated attacking a few targets and while working through their OSINT phase, they found out that their targets used a popular site called CareerBuilder
2. After completing the OSINT phase, the attackers started on pretext development. Th is led them to plan a pretext as a job seeker, who was looking to get hired at whatever role their targets were offering. They realized the tools they needed would be some maliciously encoded fi les and some realistic-looking resumes.
3. They started to plan the attacks, by answering some of those W questions.
4. They then launched the attacks by uploading their malicious documents not to the target but to the CareerBuilder website. Th e companies that posted the jobs would be notifi ed by email that there was a new applicant, and that email would contain the attacker ’ s uploaded attachments.
5. They did not follow through with any actionable reporting phase, but there is some actionable reporting on this attack thanks to some researchers at Proofpoint.

* This attack was successful because the target would get an email with an attachment from a trusted and reputable source (CareerBuilder). Consequently, the target would open the attachment without thinking. And that is exactly the goal of the malicious social engineer: to get the target to take an action that is not in their best interest without thinking through the potential dangers involved

### Do You See What I See? - 1

Regardless of how you obtain OSINT, you need to have a clear idea in mind of what you are looking for. That might seem easy to do, but it’s not as easy as it sounds. You can’t simply say, “I want all info on the target.” Every type of information has a different value, and what is valuable can change with the type of attack you are looking to launch.

#### A Real-World Example of Collecting OSINT

Why is the amount of traffic on the Internet even remotely important to understand? Well, for example, if you are looking to send a spear-phish, your goal might be to look for personal hobbies, likes, dislikes, and things the target finds valuable.

But if you are going to vish your target, then you might want to find details about the target’s job, what role the person plays in the work organization, and what kinds of internal and external resources that person would expect calls from.

If your goal is to get onsite, then you need to know whether the target would meet with people and who those people would be

You have 4.48 billion potential websites to scrape through to look for data that can be helpful. So, before you start digging in, it is important to plan your OSINT engagement. To help you establish some parameters for what you’re looking for, use the lists of questions in table.

Of course, the questions in the table only touch the surface. You can add other items about types of computers used, employee schedules, what languages are used, type of antivirus protection used, and much more.

```sample
Type of Organization Questions to Ask
 - Corporation How does the corporation use the Internet?
 - How does the corporation use social media?
 - Does the corporation have policies in place for what its people
 can put on the Internet?
 - How many vendors does the corporation have?
 - What vendors does the corporation use?
 - How does the corporation accept payments?
 - How does the corporation issue payments?
 - Does the corporation have call centers?
 - Where are headquarters, call centers, or other branches located?
 - Does the corporation allow BYOD (bring your own device)?
 - Is the corporation in one location or many locations?
 - Is there an org chart available?
```

#### Individual

```
 - What social media accounts does the person use?
 - What hobbies does the person have?
 - Where does the person vacation?
 - What are the person’s favorite restaurants?
 - What is the family history (sicknesses, businesses, and so on) of
 the person?
 - What is the person’s level of education? What did the
 person study?
 - What is the person’s job role, including whether people work
 from home, for themselves, and who they report to?
 - Are there any other sites that mention the person (maybe they
 give speeches, post to forums, or are part of a club)?
 - Does the person own a house? If yes, what are the property
 taxes, liens, and so on?
 - What are the names of the person’s family members (as well as
 any of the previously mentioned info on those people)?
```

...
