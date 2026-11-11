

## PyTorch Foundation

Minutes of the November 10, 2026 Technical Advisory Council Meeting

The Technical Advisory Council of the PyTorch Foundation (the "Foundation") met via LFX on November 10, 2026, at 7am PDT/10am EDT/4pm CEST.  The TAC meeting is scheduled every second Tuesday of every month at 7am PT/10am ET/4pm CET.  

* The meeting recording can be found here. 

**The following voting representatives attended the meeting:**   
**(11 are needed for quorum)** 

- [x] Thomas Viehmann \- TAC Chair (Lightning AI)  
- [x] Milos Puzovic \- TAC Vice Chair (ARM)  
    
- [x] Claudio Basile (Google Cloud)  
- [ ] Eikan Wang \- Ecosystem Working Group Co-Chair (Intel)  
- [x] Eyal Lantzman (Nscale)   
- [ ] Gregory Chanan (Meta)  
- [x] Jeff Daily (AMD)  
- [x] Jing Zhu (Cambricon)   
- [x] Joseph Groenenboom (Red Hat/IBM)   
- [ ] Mert Hidayetoglu (Snowflake)  
- [x] Piotr Bialecki (NVIDIA)  
- [ ] Ryan Wang (Nebius)   
- [ ] Shauheen Zahirazami (AWS)  
- [x] Shuying Sun (Shopify)  
- [ ] Tao Ma (Alibaba Cloud)   
- [x] Yikun Jiang (Huawei)  
- [ ] Weizhu Chen \- Gold Member Representative (Microsoft)  
    
- [x] Alban Desmaison \- PyTorch Project Representative (Meta)  
- [x] Jongsok Choi \- Helion Project Representative (Meta)  
- [x] Luc Georges \- Safetensors Project Representative (Hugging Face)   
- [x] Olatunji Ruwase \- DeepSpeed Project Representative (Snowflake)  
- [x] Robert Nishihara \- Ray Project Representative (Anyscale)  
- [ ] Simon Mo \- vLLM Project Representative (Inferact)

**The following alternate voting representatives attended the meeting:**  

- [x] Andrew Wafaa (ARM)  
- [ ] Ashok Emani (Intel)  
- [x] Dave Grove (Red Hat/IBM)   
- [ ] Davide Italiano (Meta)   
- [ ] Fengchun Hua (Huawei)  
- [ ] Michael Ruberry (NVIDIA)  
- [ ] Michael Voznesensky (Google Cloud)  
- [x] Niles Burbank (AMD)  
- [x] Sanghong Li (Alibaba Cloud)   
- [ ] Sundar Ranganathan (AWS)  
- [x] Richard Bian \- vLLM Project (Inferact)  
- [ ] Lysandre Debut \- Safetensors Project (Hugging Face)   
- [ ] Minjia Zhang \- DeepSpeed Project (University of Illinois Urbana-Champaign)

**The following PyTorch Working Group Leads attended the meeting:**

- [ ] Andrea Frittoli \- Multi-Cloud Working Group Lead (IBM)   
- [x] Chris Hoge \- Ecosystem Working Group Co-Chair (NVIDIA)  
- [ ] George Chellapa \- OSPO & Academic Outreach Working Group Co-Chair (NVIDIA)   
- [ ] Nikita Shulga \- Security Working Group Lead (Meta)  
- [ ] Sumantro Mukherjee \- OSPO & Academic Outreach Working Group Co-Chair (Red Hat)   
- [x] Zesheng Zong \- Accelerator Integration Working Group Lead (Huawei)

**The following personnel from The Linux Foundation attended the meeting:**

- [x] Mark Collier, PyTorch Executive Director  
- [x] Michelle Roth, Program Manager  
- [x] Regina Nkenchor, Program Manager  
- [x] Naomi Washington, Sr. Program Manager  
- [ ] Ana Jimenez, OSPO Support  
- [ ] Jennifer Bly, Marketing Director  
- [x] Ebba Simpson, Marketing  
- [ ] Deb Giles, Event Director, LF Projects  
- [x] Thanh Ha, IT  
- [ ] Ryan Aslett, IT  
- [x] Mick Tarsel, IT

**The following other individuals attended the meeting:**

* Andrey Talman (Meta)  
* Anthony Barbier (Graphcore)   
* Atharva Kshirsagar (Red Hat)   
* Chandra Mohan Singh Negi (Siemens)  
* Clement Anthonioz Blanc (Meta)   
* David vonThenen  
* Eddie Yan (NVIDIA)  
* Ion Stoica (Anyscale)   
* Jana van Greunen (Meta)   
* Jewel M (Red Hat)   
* Joshua Rosenkranz (IBM)   
* Junchen Jiang  
* Krishna Kalyan (Cloudera)   
* Ricardo Aravena (Nunchux AI)   
* Vivek Goyal (Red Hat)   
* *Yashasvi Misra*  
* Yuan Binhang (AReaL)   
* Yunbo Wang (FlagOS) 

**Call to Order**  
Thomas Viehmann shared the antitrust policy outlined in the meeting deck and called the meeting to order. Michelle Roth recorded the minutes.

**Agenda & Reminders**  
Viehmann reviewed the agenda, remaining 2026 meeting schedule, and upcoming 2027 meetings.  
                    
**Roll Call and TAC Representative List**  
Viehmann reviewed the TAC Voting Representative list, welcoming new representatives.

**Foundation Updates**

* Mark Collier highlighted that the updated Foundation-Hosted project lifecycle process is in voting, and encouraged TAC members to vote. 


  
**Q4 Project Updates**

* Ray \- Robert Nishihara  
  * Nishihara reviewed recent updates and features, noting hardening and scalability have been the main focuses.   
  * Nishihara highlighted the recent Ray Summit co-located with vLLM, noting that a full day of training was highly successful.   
  * Nishihara also noted that Ray recently started an accelerator SIG, and that KubeRay has been donated to CNCF.   
* PyTorch Project \- Alban Desmaison  
  * Desmaison highlighted over 3,000 issues closed in the last quarter, and three recent releases.   
  * Desmaison reviewed the upcoming 2.16 release and continued work on a number of areas such as the CRCR rollout.   
  * Desmaison also noted ongoing work with ExecuTorch.   
* DeepSpeed Project \- Tunji Ruwase  
  * Ruwase noted that Huawei has joined the TSC, and there has been good attendance at the monthly office hours.   
  * Ruwase reviewed the 5 recent releases, noting specific features such as parallelism.   
  * Ruwase also highlighted ongoing and upcoming blogs for Q4, and a paper at SC next week.   
* vLLM \- Richard Bian   
  * Bian presented a Q3 recap for vLLM, highlighting a stable release cadence.   
  * Bian also highlighted the Q4 roadmap has been published and the core refactor is targeted to be finished.   
  * Bian also noted work towards an OSS strategy alignment with other projects and ecosystem members, and that vLLM will be at the upcoming PyTorch Day Korea and PyTorch Day China in December.   
* Helion Project \- Jongseok Choi   
  * Choi recapped recent updates presented at PTCNA, including new backends and Helion’s megakernal compiler.   
  * Choi highlighted 4 talks/sessions at PTCNA, several recent blogs, and 4 recent releases.   
  * Choi reviewed upcoming priorities, including CuTE backend and improved megakernel compiler performance.   
* Safetensors \- Luc Georges   
  * Georges recapped recent priorities, including cuda fast path loading and hardening.   
  * Georges also reviewed future priorities. 

**Working Group Updates**

* Working Group Lifecycle and Process   
  * Viehmann presented an update on the proposed working group process and lifecycle, noting that it has been approved by the TAC.   
* CI Working Group \- Thanh Ha   
  * Ha gave an update on the CI Working Group, noting that:  
    * AWS Spend: October costs for the Foundation AWS account were \$494,000.  
    * Credits & Budget: Remaining AWS credits total roughly \$1 million.  
    * Runner Allocation: 23% allocated to Foundation account (excluding Inductor jobs).   
    * OSDC CI & Optimizations: Continuing to optimize costs, OSDC support for Windows WIP, and Nvidia GB300 now available for PyTorch CI.   
    * Costs: Ha reviewed YTD costs by architecture and hardware.   
* Ecosystem Working Group \- Chris Hoge  
  * Hoge gave an update on recent ecosystem activities, highlighting:  
    * Welcomed Joseph Groenboom as WG co-chair.   
    * New charter in progress following new WG process.   
    * Upcoming reviews: several projects are undergoing regular 6 month reviews.   
    * No new project applications this month.   
    * Ecosystem WG presentation at PTCNA went well.   
* Accelerator Integration Working Group \- Zesheng Zong  
  * Zong gave an update on recent activities, highlighting:  
    * WG in person meeting during PTCNA was well attended.   
    * Short term objectives: CRCR and test refactoring.  
    * Long term objectives: Common API for accelerators, centralized testing, and more.   
    * Cross-Repository CI Relay: several improvements including callback-rate reliability, security improvements, etc.   
* Security Working Group \- Nikita Shulga  
  * Viehmann noted that Nikita Shulga was not in attendance but Alban Desmaison was able to give an update. Desmaison noted that:   
    * 25 issues were reported in the last 30 days with 7 closed.   
    * PyTorch dependencies updated.  
    * Torch JIT script checkpoints are unsafe.   
    * Weekly triage meeting \- open to anyone  
* OSPO & Academic Outreach Working Group \- George Chellapa/Sumantro Mukherjee  
  * Viehmann noted that none of the WG chairs were in attendance but Michelle Roth was able to give an update. Roth noted that:   
    * Day Zero Academic Community Workshop: Went well, planning to hopefully have again next year.   
    * Blog Series: TinyTorch blog published, WG is asking for additional ideas/input. 

**Open Discussion**  
●      None

**Adjournment**  
Viehmann thanked all attendees for their time and participation and formally closed the meeting. 

**Next Meeting**  
The next TAC meeting is scheduled for Tuesday, December 8, 2026, at 7am PDT/10am EDT/4pm CEST. 

**Action Items**

* All TAC Members: Vote on the proposed project lifecycle update document. 

