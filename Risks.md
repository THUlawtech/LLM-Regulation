# LLM Risks

Below is a brief overview of 18 identified risks of LLMs, grouped by four main categories: **Training Data**, **The LLM Itself**, **Generated Content**, and **Others**. 


![LLM Risks](img/risks.png)

---

## A. Training Data

1. **Infringement of IP**  
   - **What It Is**: When copyrighted text, images, or other media are used in the training dataset without permission, models risk infringing on intellectual property rights.  
   - **Example**: GitHub Copilot was criticized for occasionally generating code that was identical or extremely similar to existing copyrighted code, sparking debates on fair use.  
   - **Source**:  
     - [Developers warned: GitHub Copilot code may be licensed (TechTarget, 2022)](https://www.techtarget.com/searchsoftwarequality/news/252526359/Developers-warned-GitHub-Copilot-code-may-be-licensed)

2. **Infringement of PI (Personal Information) Rights**  
   - **What It Is**: Training data might contain personal data (e.g., names, addresses, sexual orientation), breaching privacy regulations like GDPR.  
   - **Example**: Italy’s data protection authority briefly banned ChatGPT in 2023 over concerns that personal information was being collected without adequate legal basis.  
   - **Source**:  
     - [Report of the work undertaken by the ChatGPT Taskforce (EDPB, 2023)](https://www.edpb.europa.eu/our-work-tools/our-documents/other/report-work-undertaken-chatgpt-taskforce_en)

3. **Risk of Data Annotation**  
   - **What It Is**: The annotation process can expose human annotators to confidential or sensitive content (e.g., trade secrets, personal data). Annotators might also introduce bias or errors.  
   - **Example**: Annotation practices have been found to encode gender biases into AI systems. For instance, sentiment analysis models have been highlighted for biased results, where sentiments expressed by marginalized groups are labeled more negatively.  
   - **Source**:  
     - [The Forgotten Layers: How Hidden AI Biases Are Lurking in Dataset Annotation Practices (UNITE, 2024)](https://www.unite.ai/the-forgotten-layers-how-hidden-ai-biases-are-lurking-in-dataset-annotation-practices/?utm_source=chatgpt.com)

4. **Inappropriate Content**  
   - **What It Is**: Inappropriate content refers to content in the training data that may be controversial, illegal, or harmful. The risks of inappropriate content stem from various sources, including but not limited to the issues outlined in Risks 1–3, as well as potential causes such as data poisoning or unreasonable data scraping practices.  
   - **Example**:   
   - **Source**:  
     - []()

5. **Data Breach**  
   - **What It Is**: Large training sets and their accompanying metadata can be stolen or leaked—especially if cloud storage or annotation platforms are compromised. Please note that the risk mentioned here is different from the data breach in Risk 13. The latter primarily refers to the model's output containing leaked personal information, protected works of others, trade secrets, and similar content.
   - **Example**:   
   - **Source**:  
     - []()

---

## B. The LLM Itself

6. **Poor Interpretability**  
   - **What It Is**: Neural networks—especially large ones—are often “black boxes,” making it difficult to explain how they arrive at specific outputs.  
   - **Example**:   
   - **Source**:  
     - []()

7. **Discriminatory (Bias)**  
   - **What It Is**: Discriminatory of LLMs mainly stems from risks at the training data level. In addition, factors such as model design and the training process may also lead to the discriminatory.  
   - **Example**: Microsoft’s Tay chatbot quickly started to generate racist content on Twitter after interacting with trolls, demonstrating how biases can be learned and repeated.  
   - **Source**:  
     - []()

8. **Low Robustness**  
   - **What It Is**: Small changes or “adversarial” prompts can cause drastic shifts in outputs, meaning the model can fail badly outside typical scenarios.  
   - **Example**:   
   - **Source**:  
     - []()


9. **Risk of Tampering**  
   - **What It Is**: Attackers might manipulate model parameters (“model poisoning”) or training data to insert backdoors or alter behavior.  
   - **Example**: Research has demonstrated that by injecting certain trigger phrases during training, an LLM can be forced to produce malicious outputs when prompted with that trigger.  
   - **Source**:  
     - [Hidden Backdoors in Neural Networks (Gu et al., 2017)](https://arxiv.org/abs/1708.06733)

10. **Risk of Defect Propagation**  
   - **What It Is**: Errors, biases, or vulnerabilities that appear at one stage of development can propagate and amplify in subsequent versions of a model (or downstream tasks).  
   - **Example**: If a poorly vetted LLM is used to create training data for the next generation of models, the original issues can become more deeply ingrained.  
   - **Source**:  
     - [On the Dangers of Stochastic Parrots (Bender et al., 2021)](https://dl.acm.org/doi/10.1145/3442188.3445922)

---

## C. Generated Content

11. **Content Safety Risk**  
   - **What It Is**: LLMs may generate hate speech, radicalization content, or instructions for violence if prompted or misused.  
   - **Example**:   
   - **Source**:  
     - []()

12. **Data Breach (via LLM)**  
   - **What It Is**: The LLM might inadvertently reveal private or proprietary information it was trained on or that was input by other users.  
   - **Example**: Samsung employees reportedly entered sensitive source code into ChatGPT, which then became part of the service’s broader training data.  
   - **Source**:  
     - [Samsung Bans Staff’s AI Use After Spotting ChatGPT Data Leak (Bloomberg, 2023)](https://www.bloomberg.com/news/articles/2023-05-02/samsung-bans-chatgpt-and-other-generative-ai-use-by-staff-after-leak)

13. **Hallucination**  
   - **What It Is**: LLMs sometimes generate plausible-sounding but factually incorrect answers.  
   - **Example**:   
   - **Source**:  
     - []()

14. **Risks from Improper Use**  
   - **What It Is**: Malicious actors can use LLMs for phishing emails, social engineering, generating malware, or other harmful activities.  
   - **Example**: Security researchers have shown that ChatGPT-like models can assist in writing malicious code or highly personalized phishing messages.  
   - **Source**:  
     - [ChatGPT tool could be abused by scammers and hackers (BBC, 2023)](https://www.bbc.com/news/technology-67614065)

15. **Adverse Self‐Impacts**  
   - **What It Is**: Overreliance on LLMs outputs (e.g., in journalism or healthcare) might lead to skill degradation, job displacement, or mental health concerns if LLMs replace human interaction.  
   - **Example**: Some mental health app chatbots rely heavily on LLMs for conversations, raising concerns about quality of care and accountability.  
   - **Source**:  
     - [Chatbot therapy is risky. It’s also not useless. (Vox, 2023)](https://www.vox.com/technology/2023/12/14/24000435/chatbot-therapy-risks-and-potential)

---

## D. Others

16. **Computation‐Related Risks**  
   - **What It Is**: Training and running LLMs is resource‐intensive, leading to high operational costs, potential single‐vendor reliance, and large carbon footprints.  
   - **Example**: The training of GPT‐4 was estimated to produce significant CO₂ emissions, raising sustainability concerns.  
   - **Source**:  
     - [Reconciling the contrasting narratives on the environmental impact of large language models (Ren et al., 2024)](https://www.nature.com/articles/s41598-024-76682-6)

17. **Supply Chain Risks**  
   - **What It Is**: Vulnerabilities in hardware (GPUs, chips) or software libraries used to develop LLMs could compromise the entire pipeline. Shortages or geopolitical issues can disrupt hardware supply.  
   - **Example**:   
   - **Source**:  
     - []()

18. **System‐Related Risks**  
   - **What It Is**: LLMs are often deployed as part of larger systems—failure in one component (e.g., cloud servers, network infrastructure) can bring down critical services.  
   - **Example**:   
   - **Source**:  
     - []()

---

### **Summary**
LLMs present various risks categorized into four main areas: Training Data, The LLM Itself, Generated Content, and Other Factors. The refinement of risks can provide clear guidance for risk governance and serves as the foundation for managing LLMs.