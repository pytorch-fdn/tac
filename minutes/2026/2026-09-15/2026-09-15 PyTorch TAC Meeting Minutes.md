

## PyTorch Foundation

Minutes of the September 15, 2026 Technical Advisory Council Meeting

The Technical Advisory Council of the PyTorch Foundation (the "Foundation") met via LFX on September 15, 2026, at 7am PDT/10am EDT/4pm CEST.  The TAC meeting is scheduled every second Tuesday of every month at 7am PT/10am ET/4pm CET.  

* The meeting recording can be found [here](https://zoom.us/rec/share/NpzQuXwr_Z-HACMp67rRJialoWCSbExkEtOVcJiCWPWjGzZgJmctEKZl6374DPbN.2a8nH0HQ3anr1W5q). 

**The following voting representatives attended the meeting:**   
**(11 are needed for quorum)** 

- [x] Thomas Viehmann \- TAC Chair (Lightning AI)  
- [x] Milos Puzovic \- TAC Vice Chair (ARM)  
        
- [x] Claudio Basile (Google Cloud)  
- [x] Eikan Wang \- Ecosystem Working Group Co-Chair (Intel)  
- [x] Gregory Chanan (Meta)  
- [ ] Jeff Daily (AMD)  
- [x] Jing Zhu (Cambricon)   
- [x] Joseph Groenenboom (Red Hat/IBM)   
- [x] Mert Hidayetoglu (Snowflake)  
- [ ] Piotr Bialecki (NVIDIA)  
- [ ] Shauheen Zahirazami (AWS)  
- [ ] Shuying Sun (Shopify)  
- [ ] Tao Ma (Alibaba Cloud)   
- [ ] Yikun Jiang (Huawei)  
- [x] Weizhu Chen \- Gold Member Representative (Microsoft)  
        
- [ ] Alban Desmaison \- PyTorch Project Representative (Meta)  
- [x] Jongsok Choi \- Helion Project Representative (Meta)  
- [ ] Luc Georges \- Safetensors Project Representative (Hugging Face)   
- [x] Olatunji Ruwase \- DeepSpeed Project Representative (Snowflake)  
- [ ] Robert Nishihara \- Ray Project Representative (Anyscale)  
- [ ] Simon Mo \- vLLM Project Representative (Inferact)

**The following alternate voting representatives attended the meeting:**  

- [ ] Andrew Wafaa (ARM)  
- [ ] Ashok Emani (Intel)  
- [x] Davide Italiano (Meta)   
- [ ] Fengchun Hua (Huawei)  
- [ ] Michael Ruberry (NVIDIA)  
- [ ] Michael Voznesensky (Google Cloud)  
- [x] Naigang Wang (Red Hat/IBM)   
- [x] Niles Burbank (AMD)  
- [x] Sanghong Li (Alibaba Cloud)   
- [x] Sundar Ranganathan (AWS)  
- [ ] Kaichao You \- vLLM Project (Inferact)  
- [ ] Lysandre Debut \- Safetensors Project (Hugging Face)   
- [ ] Minjia Zhang \- DeepSpeed Project (University of Illinois Urbana-Champaign)

**The following PyTorch Working Group Leads attended the meeting:**

- [x] Andrea Frittoli \- Multi-Cloud Working Group Lead (IBM)   
- [x] Chris Hoge \- Ecosystem Working Group Co-Chair (NVIDIA)  
- [x] George Chellapa \- OSPO & Academic Outreach Working Group Co-Chair (NVIDIA)   
- [ ] Nikita Shulga \- Security Working Group Lead (Meta)  
- [x] Sumantro Mukherjee \- OSPO & Academic Outreach Working Group Co-Chair (Red Hat)   
- [x] Zesheng Zong \- Accelerator Integration Working Group Lead (Huawei)

**The following personnel from The Linux Foundation attended the meeting:**

- [x] Mark Collier, PyTorch Executive Director  
- [x] Michelle Roth, Program Manager  
- [ ] Regina Nkenchor, Program Manager  
- [x] Naomi Washington, Sr. Program Manager  
- [ ] Ana Jimenez, OSPO Support  
- [ ] Jennifer Bly, Marketing Director  
- [x] Ebba Simpson, Marketing  
- [ ] Deb Giles, Event Director, LF Projects  
- [x] Thanh Ha, IT  
- [ ] Ryan Aslett, IT  
- [x] Mick Tarsel, IT

**The following other individuals attended the meeting:**

* Andreas Krebbel (IBM)  
* Andrey Talman (Meta)  
* Ankit Patel (NVIDIA)   
* Anthony Barbier (Graphcore)   
* Arkadip Maitra (Red Hat)  
* Chandra Mohan Singh Negi (Siemens)  
* David vonThenen  
* Eddie Yan (NVIDIA)  
* Jana van Greunen (Meta)   
* Jewel M (Red Hat)  
* Joe Spisak (Reflection AI)   
* Joshua Rosenkranz (IBM)   
* Nayan Bushan Kanganahalli Nagabhushana (Red Hat)   
* Pruthvi Madugundu (AMD)   
* Ricardo Aravena (Snowflake)  
* Vivek Goyal (Red Hat)   
* Xiaoya Xia (CHAOSS/Ant Group)  
* Yuan Binhang (AReaL) 

**Call to Order**  
Thomas Viehmann shared the antitrust policy outlined in the meeting deck and called the meeting to order. Michelle Roth recorded the minutes.

**Agenda & Reminders**  
Viehmann reviewed the agenda and upcoming 2026 meeting schedule, highlighting the upcoming TAC meetup scheduled for PyTorch Conference North America.   
                    
**Roll Call and TAC Representative List**  
Viehmann reviewed the TAC Voting Representative list, welcoming Jing Zhu as Cambricon’s new representative, and Davide Italiano as the new alternate representative for Meta. 

**Foundation Updates**

* Mark Collier announced two new Foundation members: Cambricon, an AI accelerator company based in China, joined as a Platinum member, and Ant Group joined as a Gold member. Cambricon representative Jing Zhu introduced himself to the TAC. Collier also noted that the inaugural PyTorch Conference China exceeded its attendance goal and provided valuable opportunities to connect with the global PyTorch community.  
*  Thomas Viehmann introduced a working group process document, adapted from an existing Linux Foundation template, outlining how to establish and retire a working group. Viehmann asked TAC members to review the document and provide feedback, with a vote on adoption planned for the next meeting.

**Working Group Updates**

* CI Working Group \- Thanh Ha   
  * Ha gave an update on the CI Working Group, noting that:  
    * AWS Spend: August costs reached $516,000, within the $500,000 monthly target.  
    * Credits & Budget: Remaining AWS credits total just over $1 million, representing approximately two months of budgeted spend.  
    * Runner Allocation: Runner allocation on the Foundation account was set to 15% of jobs, excluding inductor jobs, subject to ongoing adjustment.  
    * OSDC CI & Optimizations: The team resolved a NAT gateway misconfiguration that was inflating data transfer costs and rebalanced control-plane pod placement, enabling a reduction in base node size and the use of cheaper instances. Ha noted that CI usage continues to trend upward and that the team is investigating the cause.  
    * Reporting: Ha introduced a new auto-generated HTML report replacing the prior manual CI cost and runtime spreadsheets, with public hosting targeted for next month.  
* Ecosystem Working Group \- Eikan Wang  
  * Wang gave an update on recent ecosystem activities, highlighting:  
    * Project Admissions: The WG accepted three new projects into the ecosystem: TorchServe, TorchL, and Zeus.  
    * Active Applications: One new application, an on-device inference framework, is pending intake review; other applications remain under review.  
    * Future Workstreams: The WG is drafting a new working group charter, finalizing an ecosystem survey, and developing skills and review guidelines to make the evaluation process more consistent and repeatable. The WG is also preparing a talk for the upcoming PyTorch Conference.  
* Accelerator Integration Working Group \- Zesheng Zong  
  * Zong gave an update on recent activities, highlighting:  
    * CRCR Progress: LSL level promotion criteria were finalized, and a per-record promotion/demotion panel shipped. Database, PR, and nightly dashboard views were added along with a file/test drill-down UI and artifact URL rendering. Several L3 accuracy bugs were also fixed.  
    * External CI: Updates were made to external CI integration, including multi-issue OIDC support and updated CI provider configuration, with VRM registration completed.  
    * Test Refactoring: Only a small number of files were merged this month; most pull requests have moved into final review, pending maintainer sign-off.  
* Security Working Group   
  * Viehmann gave an update on security, noting:  
    * Security Advisories: Nikita Shulga was not in attendance; the security update slide had been refreshed following the working group's meeting the prior week. A constant flow of security issues continues to be reported and processed in an orderly fashion, with no critical issues to report.  
* OSPO & Academic Outreach Working Group \- Ana Jimenez/George Chellapa/Sumantro Mukherjee  
  * Mukherjee gave an update on the OSPO & Academic Outreach Working Group, highlighting:  
    * Day Zero Event: The Day Zero event at the PyTorch Conference has been finalized, with an agenda and registration link forthcoming. A call for projects will be issued via blog post, inviting community project submissions for consideration as event presentations.  
    * Publications: A blog post in collaboration with Harvard University on Tiny Torch is forthcoming.

**Open Discussion**  
●      Viehmann noted that the TAC voted to reject two project applications following July and August presentations, and invited feedback on the experience, noting that ONNX's contact had described the invitation-then-rejection sequence as a confusing experience.  
●      Weizhu Chen suggested that invitation and acceptance be explicitly decoupled going forward, and that accept/reject rationale should be documented, raising the question of whether such rationale should be published or kept internal.  
●      Milos Puzovic suggested making the comment field required when TAC members vote, to make it easier to gather structured feedback. Michelle Roth agreed to look into whether LFX voting can support a required comment field, and noted the Foundation continues to solicit feedback by email after votes, offering anonymity to commenters.  
●      Mark Collier noted that, as the Foundation fields more inbound interest from fast-growing projects, there is a perceived risk that adding hosted projects could crowd out resources for flagship projects like PyTorch. Collier reiterated that developing a more granular project lifecycle, with intermediate stages beyond simply "hosted" and "not hosted," would let the Foundation say yes to strong projects without that tradeoff, and would help prospective projects better gauge fit before applying.  
●      Chris Hoge suggested revisiting the Ecosystem Working Group's original scope as an incubation space and stepping stone toward full Foundation project status, a role the group had de-scoped earlier in the year, and proposed reintroducing it as part of the group's in-progress charter rewrite.  
●      Joe Spisak agreed with Hoge, noting that the ecosystem tier should stay broad, lightweight, and low-friction for early-stage projects, while the highest-quality, most mature projects graduate toward full Foundation hosting. Spisak and Collier discussed that the value proposition for joining the Foundation, beyond visibility such as a blog post or conference mention, is not always clear to prospective projects and needs to be better articulated.  
●      Collier noted that ONNX and another AI project, discussed by Joe Spisak, have expressed hesitation about joining the Foundation due to concerns about added process slowing development, though the Foundation's neutral, long-term-committed positioning still carries value for high-quality projects, particularly as trust in software provenance becomes more important with the rise of AI-assisted coding.

**Adjournment**  
Viehmann thanked all attendees for their time and participation and formally closed the meeting. 

**Next Meeting**  
The next TAC meeting is scheduled for Tuesday, October 13, 2026, at 7am PDT/10am EDT/4pm CEST. 

**Action Items**

* All TAC Members: Review and provide feedback on the proposed working group process document, with the aim of voting to adopt it at the next meeting (October 13, 2026).  
* Thanh Ha: Host the auto-generated CI cost and runtime reports on a web page for public access by next month.  
* Michelle Roth: Investigate whether LFX voting can be configured to require comments on votes, to help gather feedback on project acceptance/rejection.  
* Mark Collier: Clarify and articulate the value proposition for projects considering joining the PyTorch Foundation, addressing concerns about bureaucracy and benefits.

