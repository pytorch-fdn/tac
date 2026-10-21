

## PyTorch Foundation

Minutes of the October 13, 2026 Technical Advisory Council Meeting

The Technical Advisory Council of the PyTorch Foundation (the "Foundation") met via LFX on October 13, 2026, at 7am PDT/10am EDT/4pm CEST.  The TAC meeting is scheduled every second Tuesday of every month at 7am PT/10am ET/4pm CET.  

* The meeting recording can be found [here](https://zoom.us/rec/share/9_YIKvR9ybQZs2h0_seh9DlbM1IVDbYBkcTj23ZtlVNDB0wFw-yjyqGLSlNcutCb.naF0dCDVRnYAs3Vr). 

**The following voting representatives attended the meeting:**   
**(11 are needed for quorum)** 

- [x] Thomas Viehmann \- TAC Chair (Lightning AI)  
- [x] Milos Puzovic \- TAC Vice Chair (ARM)  
        
- [x] Claudio Basile (Google Cloud)  
- [ ] Eikan Wang \- Ecosystem Working Group Co-Chair (Intel)  
- [x] Gregory Chanan (Meta)  
- [x] Jeff Daily (AMD)  
- [ ] Jing Zhu (Cambricon)   
- [x] Joseph Groenenboom (Red Hat/IBM)   
- [x] Mert Hidayetoglu (Snowflake)  
- [x] Piotr Bialecki (NVIDIA)  
- [x] Shauheen Zahirazami (AWS)  
- [x] Shuying Sun (Shopify)  
- [x] Tao Ma (Alibaba Cloud)   
- [x] Yikun Jiang (Huawei)  
- [x] Weizhu Chen \- Gold Member Representative (Microsoft)  
        
- [x] Alban Desmaison \- PyTorch Project Representative (Meta)  
- [ ] Jongsok Choi \- Helion Project Representative (Meta)  
- [x] Luc Georges \- Safetensors Project Representative (Hugging Face)   
- [x] Olatunji Ruwase \- DeepSpeed Project Representative (Snowflake)  
- [ ] Robert Nishihara \- Ray Project Representative (Anyscale)  
- [ ] Simon Mo \- vLLM Project Representative (Inferact)

**The following alternate voting representatives attended the meeting:**  

- [x] Andrew Wafaa (ARM)  
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

- [ ] Andrea Frittoli \- Multi-Cloud Working Group Lead (IBM)   
- [x] Chris Hoge \- Ecosystem Working Group Co-Chair (NVIDIA)  
- [x] George Chellapa \- OSPO & Academic Outreach Working Group Co-Chair (NVIDIA)   
- [ ] Nikita Shulga \- Security Working Group Lead (Meta)  
- [x] Sumantro Mukherjee \- OSPO & Academic Outreach Working Group Co-Chair (Red Hat)   
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

* Andreas Krebbel (IBM)  
* Andrey Talman (Meta)  
* Atharva Kshirsagar (Red Hat)   
* Chandra Mohan Singh Negi (Siemens)  
* Clement Anthonioz Blanc (Meta)   
* Dmitry Rogozhkin   
* Eddie Yan (NVIDIA)  
* Ion Stoica   
* Joshua Rosenkranz (IBM)   
* Morrison Turnansky (Red Hat)   
* Ricardo Aravena (Snowflake)  
* Tao Zhang (Dell)   
* Vivek Goyal (Red Hat)   
* Yashasvi Misra  
* Yuan Binhang (AReaL) 

**Call to Order**  
Thomas Viehmann shared the antitrust policy outlined in the meeting deck and called the meeting to order. Michelle Roth recorded the minutes.

**Agenda & Reminders**  
Viehmann reviewed the agenda and upcoming 2026 meeting schedule, highlighting the upcoming TAC meetup scheduled for PyTorch Conference North America.   
                    
**Roll Call and TAC Representative List**  
Viehmann reviewed the TAC Voting Representative list.

**Foundation Updates**

* Mark Collier introduced a discussion on the types of projects the TAC would like to prioritize for Foundation hosting, noting that the Foundation became multi-project last year with the addition of vLLM, DeepSpeed, and Ray, and that Safetensors and Helion have been added so far this year. Collier noted that the TAC voted on two widely adopted projects, ONNX and AReaL, that were not approved, and said that building consensus on the right fit would help the group steer prospective projects before applications arrive  
* Ion Stoica identified reinforcement learning and data processing as areas with reasonably mature or soon-to-be-mature candidates, citing SkyRL and verl (noting verl is more mature but heavy) for RL, and DataTrove (Hugging Face) and NeMo Curator for data processing. He identified agentic loops and evolutionary algorithms (e.g., SkyDiscover, OpenEvolve) as an area to watch, but noted it is fragmented and fast-moving. He also cited Megatron and TorchTitan for distributed training and Dynamo (NVIDIA) for distributed inference, noting that NVIDIA invests heavily in open source and may have other potential projects. Collier added that Mooncake has come up a few times and is currently part of the ecosystem.  
* Weizhu Chen suggested the TAC consider sandboxes and environments used for RL, automation of model training, and on-device training and inference, noting it is unclear which projects will become popular.  
* Viehmann noted that the Foundation is not trying to pick winners and said he would prioritize widely used but often unseen "plumbing" projects, such as quantization projects (including those implementing quantization for vLLM). He added that, if there is consensus, he would be inclined to revisit ONNX.   
* Sundar Ranganathan suggested the TAC consider disaggregated inference, noting growing customer interest in higher-throughput inference workloads, and mentioned SGLang. He asked how an NVIDIA-owned project such as Dynamo would work under the Foundation. Ranganathan will poll his team on growing trends and bring back candidates. Collier agreed this is a strong trend for the Foundation to participate in.  
* In response to a question from Alban Desmaison, Viehmann clarified that the governing board has made a strategic decision to grow the number of hosted projects, that this does not automatically bring compute resources or other resources, and that the TAC's role is to decide which projects are a good fit and how to bring them in, not whether to grow. Collier added that the board has not set a target number of projects or a deadline.  
* Collier reviewed the latest iteration of the Foundation-Hosted Project Lifecycle Process, noting it has been reduced from 20-plus pages to 3 and consolidated, with Desmaison's help. The process moves from a single "hosted" stage to two stages, incubated and graduated, plus an archived state. The TAC would decide by majority vote which projects enter as incubated; graduation would require approval by both the TAC and the governing board. Collier noted this would make it easier to bring in projects that are not yet at PyTorch, vLLM, or Ray scale.   
* Stoica raised a concern that accepting more projects could dilute the Foundation's focus and leave it with many inactive projects, and asked that the process include a clear way to remove projects and how it differs from other foundations. Collier acknowledged the risk and described built-in mitigations: the archive state, regular project updates to the TAC to assess health and activity, and discerning judgment up front, since no project enters without a TAC majority vote. Stoica recommended against using the number of projects as a proxy for the Foundation's strength, citing experience at the Apache Foundation, and Collier agreed. Viehmann noted that the TAC is responsible for balancing which projects to accept and which to archive.  
* Viehmann proposed giving the TAC a week to review the newest version and discuss live at PTCNA, with a vote to follow. Discussion can also continue in the TAC Slack channel. 

**Working Group Updates**

* Working Group Lifecycle and Process   
  * Viehmann presented a short (about two and a half pages) working group process document describing how to propose, charter, and close a working group. Forming a working group does not provide compute resources; it provides administrative support. Proposers articulate purpose, goals, non-goals, and proposed deliverables in a charter based on a template and submit it to the TAC, which votes to start a working group, checks on working groups periodically, and closes them when goals are achieved or they are no longer needed. Existing working groups continue as they are.   
  * Viehmann proposed an offline vote on the current wording and asked members to vote yes if it is good enough, noting it can be revised later. Joseph Groenenboom asked that the vote happen soon, ideally before the conference, so there is an answer for people asking about forming working groups. Roth will send the vote out asynchronously after the meeting and noted a couple of terms that need consensus.  
* CI Working Group \- Thanh Ha   
  * Ha gave an update on the CI Working Group, noting that:  
    * AWS Spend: September costs for the Foundation AWS account were \$452,000, under the usual \$500,000 target, due to CI efficiency optimizations made in the last couple of weeks.   
    * Credits & Budget: Remaining AWS credits total roughly \$1 million, representing approximately two months of budgeted spend.   
    * Runner Allocation: Because of the cost reduction, the percentage of jobs allocated to the Foundation account was increased to 20%.   
    * OSDC CI & Optimizations: The team continues to optimize costs and cluster sizing on the new CI system and is working on a runner allow-list feature to give more control over which runners run on the LF fleet versus the Meta fleet. The team also tuned instance-type priorities for G4DN, G5, and G6 on the LF fleet to select more efficient instance sizes, and is already seeing a noticeable reduction in overhead costs.  
    * Reporting: The web-based CI reports are now hosted at cireports.pytorch.org and require an LFID login. TAC members should have access, and Ha asked anyone whose LFID does not work to contact him. The site contains the snapshot data behind the monthly charts.   
    * Runtime & Growth Metrics: Combined hardware runtime decreased in September. Alban Desmaison noted that Meta is working to de-duplicate jobs and expects the trend to continue. Ha introduced a CI growth metrics slide showing year-over-year growth of 66% in PRs opened, over 200% in jobs run, 68% in unique contributors, over 100% in runtime hours, and 40% in hours per PR. Ha invited requests for additional metrics for next month's slides.  
* Ecosystem Working Group \- Chris Hoge  
  * Hoge gave an update on recent ecosystem activities, highlighting:  
    * Project Admissions: The WG accepted two projects, LitData and XGrammar, and renewed Torch Distill.  
    * Active Applications: One application is under review, LiteRT (Google's open-source runtime for deploying PyTorch models on edge, mobile, desktop, web, and embedded devices). No other projects are under review.   
    * Future Workstreams: The WG is updating its charter to align with the new working group process and project lifecycle. Ecosystem WG membership is no longer required for projects to advance, so the WG is working to position the ecosystem so that participation is not mistaken for Foundation project status. A draft mission statement describes the ecosystem as a low-barrier way to recognize open, community-oriented projects outside the Foundation, whether as a stepping stone or an endpoint. Hoge asked for guidance from Foundation and TAC leadership on positioning and messaging. An ecosystem project survey is also underway, and Hoge and Joseph Groenenboom will present on the Ecosystem Working Group at the conference.  
* Accelerator Integration Working Group \- Zesheng Zong  
  * Zong gave an update on recent activities, highlighting:  
    * CRCR Progress: L3 gating is now live; whether a backend can reach L3 depends on its overall pass rate and time at L2. While a demotion PR is open, new upstream check runs stop being sent. DataSync can open demotion PRs automatically, and downstream backends can change verdicts through callbacks to indicate whether a failure comes from upstream changes or the backend. Backends can now choose to participate in pull request events, nightly events, or both; nightly-only backends are excluded from PR views, dispatch, and the L3 view.   
    * Dr. CI & Data Reliability: Dr. CI now shows L3 results only when a PR has the CRCI label, so shadow runs without the label no longer appear as PR checks. Fixes were made to fallback ingestion, Buildkite mappings, and UTC timestamps, making data and health diagnosis more reliable.   
    * Test Refactoring: Over 100 files were updated since the last meeting, and the team is focused on the next round of initial reviews.   
    * Conference: An in-person working group meeting is planned during the conference. Zong will post the time and meeting room in the working group channel once confirmed.  
* Security Working Group \- Nikita Shulga  
  * Viehmann noted that Nikita Shulga was not in attendance and deferred the security update to the next meeting in the interest of time.  
* OSPO & Academic Outreach Working Group \- George Chellapa/Sumantro Mukherjee  
  * Chellapa gave an update on the OSPO & Academic Outreach Working Group, highlighting:  
    * Day Zero Academic Community Workshop: The workshop is the following Monday, with lightning talks from academic projects using PyTorch or other hosted projects, followed by a session helping research projects become more community-enabled. Registration is open and the group is still seeking volunteers to help with the workshop portion.   
    * Blog Series: The working group started a blog series highlighting academic projects using PyTorch, and the first post went live last week. Chellapa asked that anyone aware of academic projects to feature contact him or Sumantro Mukherjee.

**Open Discussion**  
●      None

**Adjournment**  
Viehmann thanked all attendees for their time and participation and formally closed the meeting. 

**Next Meeting**  
The next TAC meeting is scheduled for Tuesday, November 10, 2026, at 7am PDT/10am EDT/4pm CEST. 

**Action Items**

* Michelle Roth: Send the working group process document out for an asynchronous TAC vote after the meeting.   
* All TAC Members: Vote on the proposed working group process document.   
* All TAC Members: Review the latest Foundation-Hosted Project Lifecycle Process document and continue discussion at PTCNA and in the TAC Slack channel.   
* Sundar Ranganathan: Poll his team on growing trends in disaggregated inference and bring back candidate projects to the TAC.   
* Thanh Ha: Continue optimizing CI costs and cluster sizing, and continue work on the runner allow-list feature; add any additional metrics requested by TAC members to next month's slides.  
* Chris Hoge: Update the Ecosystem Working Group charter in alignment with the new working group process and project lifecycle, and seek guidance from Foundation and TAC leadership on ecosystem positioning and messaging.   
* Zesheng Zong: Post the in-person Accelerator Integration Working Group meeting time and room in the working group channel once confirmed.   
* All TAC Members: Volunteer for the Day Zero Academic Community Workshop and suggest academic projects for the blog series by contacting George Chellapa or Sumantro Mukherjee.

