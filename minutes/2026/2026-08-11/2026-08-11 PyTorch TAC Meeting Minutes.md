

## PyTorch Foundation

Minutes of the August 11, 2026 Technical Advisory Council Meeting

The Technical Advisory Council of the PyTorch Foundation (the "Foundation") met via LFX on August 11, 2026, at 7am PDT/10am EDT/4pm CEST.  The TAC meeting is scheduled every second Tuesday of every month at 7am PT/10am ET/4pm CET.  

* The meeting recording can be found [here](https://zoom.us/rec/play/ccFX-jgFonIOxWvvBV61VGpUXfhoX1EiLsiHM1IkCLBgJWCj_gHlJIUUSzuwNY-xC4CzQHpFux-Q7_Tx.eblpS8K6VCSHFTFi?accessLevel=meeting&canPlayFromShare=true&from=share_recording_detail&continueMode=true&oldStyle=true&componentName=rec-play&originRequestUrl=https%3A%2F%2Fzoom.us%2Frec%2Fshare%2FxA-04rq8N26oYD_HT_V1bKW2leqD7KbsifO0r651FClDlVt-dka-ut85_GclPnMQ.iDPFJd0Pe7pSo2Dw). 

**The following voting representatives attended the meeting:**   
**(12 are needed for quorum)** 

- [ ] Thomas Viehmann \- TAC Chair (Lightning AI)  
- [ ] Milos Puzovic \- TAC Vice Chair (ARM)  
        
- [x] Claudio Basile (Google Cloud)  
- [x] Eikan Wang \- Ecosystem Working Group Co-Chair (Intel)  
- [ ] Gerred Dillon (Nscale)   
- [x] Gregory Chanan (Meta)  
- [x] Jeff Daily (AMD)  
- [x] Joseph Groenenboom (Red Hat/IBM)   
- [x] Mert Hidayetoglu (Snowflake)  
- [x] Piotr Bialecki (NVIDIA)  
- [x] Shauheen Zahirazami (AWS)  
- [x] Shuying Sun (Shopify)  
- [ ] Tao Ma (Alibaba Cloud)   
- [x] Yikun Jiang (Huawei)  
- [x] Weizhu Chen \- Gold Member Representative (Microsoft)  
        
- [x] Alban Desmaison \- PyTorch Project Representative (Meta)  
- [x] Jongsok “James” Choi \- Helion Project Representative (Meta)  
- [x] Luc Georges \- Safetensors Project Representative (Hugging Face)   
- [x] Olatunji Ruwase \- DeepSpeed Project Representative (Snowflake)  
- [ ] Robert Nishihara \- Ray Project Representative (Anyscale)  
- [ ] Simon Mo \- vLLM Project Representative (Inferact)

**The following alternate voting representatives attended the meeting:**  

- [x] Andrew Wafaa (ARM)  
- [x] Ashok Emani (Intel)  
- [ ] Fengchun Hua (Huawei)  
- [ ] Hamid Shojanazeri (Meta)   
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
- [x] Jordan Conway, IT  
- [x] Mick Tarsel, IT

**The following other individuals attended the meeting:**

* Andreas Fehlner (ONNX)   
* Andrew Caples (Meta)   
* Andrey Talman (Meta)  
* Ankit Patel (NVIDIA)   
* Arkadip Maitra (Red Hat)  
* Chandra Mohan Singh Negi (Siemens)  
* Clement Anthonioz Blanc (Meta)  
* David vonThenen  
* Eddie Yan (NVIDIA)  
* Ganesan Ramalingam (Microsoft)   
* Ion Stoica (Anyscale)  
* Jana van Greunen (Meta)   
* Jewel M (Red Hat)  
* Joe Spisak (Reflection AI)   
* Joshua Rosenkranz (IBM)   
* Mansi Agarwal (Red Hat)   
* Priya Sethuraman (NVIDIA)   
* Ricardo Aravena (Snowflake)  
* Sanskar Prasad (Red Hat)   
* Souvik Hazra (Red Hat)   
* Subin George (Red Hat)   
* Vivek Goyal (Red Hat)   
* Xiaoya Xia (CHAOSS/Ant Group)  
* Yashasvi Misra (Pure Storage) 

**Call to Order**  
Michelle Roth shared the antitrust policy outlined in the meeting deck and called the meeting to order, noting that Thomas Viehmann and Milos Puzovic are out of office. Roth recorded the minutes.

**Agenda & Reminders**  
Roth reviewed the agenda and upcoming 2026 meeting schedule, highlighting proposed TAC meetups scheduled for PyTorch Conferences China and North America (for TAC members only) and the PyTorch Conference Community Night at PTC China that will be open to anyone to join.   
                    
**Roll Call and TAC Representative List**  
Roth reviewed the TAC Voting Representative list, welcoming Gerred Dillon as Nscale’s new representative, Joseph Groenenboom as the new voting representative for IBM and Naigang Wang as the new alternate representative for IBM. 

**Foundation Updates**

* Mark Collier reviewed the Foundation’s core priorities and goals for 2026:  
  * Multi-project evolution: Evolving organizational charters and project lifecycle frameworks to support scaling and resource allocation.  
  * CI Infrastructure: Managing the highly strategic, complex, and costly CI infrastructure (specifically PyTorch).  
  * Events: Organizing the upcoming PyTorch Conferences, PyTorch Days, and other community gatherings (such as NeurIPS).  
* Collier announced that Matt White has departed the Linux Foundation, thanking him for his instrumental contributions to establishing the TAC and growing the Foundation. Collier introduced Mick Tarsel as a newly hired CI Engineer at the Linux Foundation, bringing infrastructure experience from IBM and Red Hat. Collier also noted a job posting for a Senior Director of Community.  
* Michelle Roth reviewed the process of updating the PyTorch Foundation lifecycle policy, noting that the LF legal team recommended a simpler approach. Roth outlined three options under consideration: the current draft version 3.4, an ASWF-based policy, and the standard LF standard template. Yashasvi Misra and Alban Desmaison volunteered to assist with drafting.  
* The committee discussed project lifecycle simplification. Joseph Spisak questioned the Foundation’s optimization goals regarding project quantity versus quality. Collier clarified that the foundation aims to avoid a "long tail" of inactive projects. Alban Desmaison noted that the target is hosting the majority of influential open-source AI projects through a balance of establishing relations with major projects and incubating early-stage projects. Roth proposed holding a dedicated working session to review options and draft a policy for an upcoming TAC vote, with follow-ups in the TAC Slack channel.  
* Roth updated the TAC on the Ambassador Program, noting that a new cohort is undergoing reviewer evaluation with acceptance notifications planned for September. The program is expanding into new regional communities where the foundation previously lacked a presence.

**Foundation-Hosted Project Application: ONNX**

* Andreas Fehlner presented the ONNX application to become a Foundation-hosted project within the PyTorch Foundation, alongside steering committee member G. Ramalingam. Fehlner reviewed ONNX as an open, vendor-neutral standard for machine learning model interoperability and intermediate representation. Fehlner outlined ONNX's governance structure, including annual community elections, special interest groups (SIGs), and working groups focusing on generative AI, safety-critical systems, and probabilistic programming. Fehlner highlighted PyTorch as the primary source of ONNX exports and noted that joining the Foundation would increase visibility and foster collaboration.  
* Alban Desmaison requested clarification regarding the scope of the application. Fehlner confirmed that the application covers the ONNX specification and its associated converters and tooling under the ONNX GitHub organization, which is separate from Microsoft's ONNX Runtime.  
* Desmaison asked how the ONNX specification fits into a modern PyTorch stack, where training and inference are increasingly Python-centric (e.g., vLLM and SGLang) and edge deployment utilizes ExecuTorch. G. Ramalingam explained that ONNX is similar to ExecuTorch as they share a common FX-based exporter. G. Ramalingam added that ONNX acts as a serialized representation that allows PyTorch models to be deployed on any backend supporting the ONNX format. Fehlner provided examples from safety-critical and regulated industries where production systems rely on legacy backends (such as OpenVINO 2021.4) that are difficult to update, making a stable, backward-compatible format like ONNX a trusted path for deploying models trained in modern PyTorch.  
* Claudio Basile added that ExecuTorch is not the sole runtime for edge devices, citing LiteRT and ONNX as alternatives. Basile suggested that the TAC should present edge solutions more holistically, beginning with Torch Export as the common entry point. Desmaison agreed, noting that the PyTorch core equivalent to the ONNX specification is the exported program spec (Torch Export), with ONNX functioning as a downstream consumer of the exported program.  
* Roth noted that the next step would be a formal vote on the ONNX application, which will be sent out via LFX post-meeting.

**Working Group Updates**

* CI Working Group \- Thanh Ha   
  * Ha gave an update on the CI Working Group, noting that:  
    * AWS Spend: July costs reached $747,000. Ha reminded the TAC that higher spending was permitted in July to offset underspending in May and June caused by the OSDC migration.  
    * Credits & Budget: Remaining AWS credits exceed $1 million, representing approximately two months of budgeted spend. The target spend for August is back to the baseline of $500,000.  
    * Runner Allocation: Runner allocation on the Foundation account has been set to 25% of jobs, excluding inductor jobs, subject to ongoing adjustments.  
    * OSDC CI & Optimizations: Cluster sizing and cost optimizations are ongoing. Recent improvements to OSDC runner utilization yielded a 5% efficiency increase. The legacy multi-cloud working group dev cluster was successfully decommissioned, reclaiming associated spend. Ha presented the 12-month trend and cost breakdowns.  
* Ecosystem Working Group \- Chris Hoge  
  * Hoge gave an update on recent ecosystem activities, highlighting:  
    * Project Admissions: EWG experienced increased velocity, accepting TokenSpeed (a PyTorch-based LLM inference engine optimized for agentic workloads) and Shepard Model Gateway (SMG) from LightSeek, FiftyOne (dataset and computer vision model tool), and VisualTorch.  
    * Active Applications: Applications for TorchServe, Deep Survival Analysis, and NeuralDBG are active, with NeuralDBG scheduled for an intake review.  
    * Remediation: Zeus (energy consumption measurement) remains in remediation as they establish governance and update project metrics.  
    * Project Continuity: The WG has had difficulty contacting representatives for torchao. Alban Desmaison noted that Christian is actively maintaining the project and advised reaching out via Slack rather than GitHub. Desmaison agreed to follow up.  
    * Future Workstreams: WG is drafting a new working group charter for TAC approval, finalizing a member needs survey, developing repeatable review guidelines, and preparing for an accepted presentation at the PyTorch Conference.  
* Accelerator Integration Working Group \- Zesheng Zong  
  * Zong gave an update on recent activities, highlighting:  
    * Platform Page Launch: The Additional Compute Platforms page is live on the PyTorch website, featuring content for MQ and Xview.  
    * WG Governance: The admission process, application report, and working group charter are finalized. Roth will send out the WG charter vote post-meeting.  
    * CRCR Improvements: Progress includes launching a metrics page, a PR board dashboard, and L3/L4 grid filtering. Failure reasons are now surfaced in PR CI comments.  
    * Periodic CI: Callback handlers, shell validators, and action inputs have been implemented.  
    * L4 Workflows: The L4 blocking workflow is in progress, with active discussions and test implementations underway. Downstream CI events were modified to trigger only on merged PRs, and the CSR renaming was completed.  
    * Test Refactoring: The refactoring has covered 270 files, with over 130 PRs in initial review and 7 in final review. Zong noted the WG will focus on initial reviews to accelerate progress.  
* Security Working Group   
  * Desmaison gave an update on security, noting:  
    * Infrastructure Security: The group identified and resolved vulnerabilities associated with a couple of insecure bots. Infrastructure patching remains ongoing.  
    * Security Advisories: The team continues to manage an influx of security advisories, mostly focused on serialization formats and safe arguments, with no critical issues to report.  
* OSPO & Academic Outreach Working Group \- Ana Jimenez/George Chellapa/Sumantro Mukherjee  
  * Chellapa gave an update on the OSPO & Academic Outreach Working Group, highlighting:  
    * WG Meetings: The group meets monthly on the fourth Wednesday at 8:00 AM PT.  
    * Publications: The first blog post has been submitted for review. The working group finalized a blog post style guide.  
    * Curriculum Workstream: The Curriculum Development Workstream Charter is live and available for TAC review.  
    * Academic Initiatives: The group is planning a PyTorch meetup for academic institutions. Additionally, the group is conducting outreach through the Curious Network to determine how the foundation can support faculty, starting with the Curious Network and expanding to other universities in the Asia-Pacific region.

**Open Discussion**  
No open discussion was presented. 

**Adjournment**  
Roth thanked all attendees for their time and participation and formally closed the meeting. 

**Next Meeting**  
The next TAC meeting is scheduled for Tuesday, September 15, 2026, at 7am PDT/10am EDT/4pm CEST. 
