---
layout:
  width: default
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: false
  pagination:
    visible: true
  metadata:
    visible: false
  tags:
    visible: true
  actions:
    visible: false
  anchors:
    visible: false
---

# DPIA Questionnaires

**DPIA Questionnaires** help organizations assess data privacy risks across processes, systems, and vendor integrations. Question sets created here can be mapped directly to Record of Processing Activities (RoPA), Sharing Partners, and Integration assessments.

This helps organizations maintain a consistent and traceable approach to privacy risk assessments across business processes and domains.

A default Questionnaire is provided as a reference. To manage DPIA Questionnaire, in the left menu go to **Platform** > **DPIA Questionnaires**.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/DPIA Questionnaires - Default.png" alt=""><figcaption></figcaption></figure></div>

### Creating a new DPIA Questionnaire set

* Select **+ Create New Set** in the top-right corner.
* In the **Create New Set** dialog box,
  * Enter a unique title for the question set (e.g., `PrimeBank_questionnaires`), and&#x20;
  * A brief summary describing the purpose or scope of this questionnaire set.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/DPIA - Create new set.png" alt=""><figcaption></figcaption></figure></div>

Select **Save** to create the set and open the DPIA editor.

Now, structure it into sections and assign weighted risk values.

**Adding Sections and Questions**:

* Use **+ Add Section** and add sections.
* Now, expand the target section and click **+ Add question**.
* Enter the risk question and set the risk parameters for each question:
  * **Yes Weightage %**: Specify the risk percentage assigned if the answer is "Yes".
  * **No Weightage %**: Specify the risk percentage assigned if the answer is "No".
  * **Default Answer**: Select Yes or No to establish the default baseline response.

Similarly, add all the risk assessment questions in all the sections.&#x20;

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/DPIA - Adding sections &#x26; questions.png" alt=""><figcaption></figcaption></figure></div>

> Alternate options to add questions:
>
> *   You can use **Generate Risk Questions with AI** option to generate questions by asking what questions you need:<br>
>
>     <div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/DPIA - Generate with AI.png" alt="" width="563"><figcaption></figcaption></figure></div>
> * You can use **Import** option to upload the questionnaire.

Use **Move up** (![](<../../../.gitbook/assets/Move up icon.png>)) and **Move down** (![](<../../../.gitbook/assets/Move down icon.png>)) actions to alter the order of the sections or the questions in a section. You can delete questions or sections if they are no longer required.

Then, select **Save Changes** to save the questionnaire.

### Mapping DPIA Questionnaires to Assessment Types

In TrustWiser, Data Protection Impact Assessments (DPIAs) are integrated into specific privacy workflows to evaluate risk at different operational touchpoints:

* **RoPA (Record of Processing Activities)**: Assessments linked to internal processing activities across business departments (e.g., automated credit scoring, HR onboarding, customer data analytics).
  * _Focus_: Legal basis for processing, data retention, data minimization, and customer privacy rights.
* **Integration**: Assessments triggered when integrating systems, core banking platforms, APIs, or cloud services.
  * _Focus_: Data security in transit/at rest, cross-system data flows, technical safeguards, and API access controls.
* **Sharing Partner / Third-Party**: Assessments for evaluating external vendors, credit reference bureaus, or partner institutions that process customer data.
  * _Focus_: Data Processing Agreements (DPAs), cross-border data transfers, and third-party security postures.

As standard questionnaire fails to capture the specific risks of different operational activities, mapping DPIA question sets ensures that each privacy assessment uses questions specifically tailored to its operational context. Mapping automatically delivers the right risk scoring and regulatory criteria for every scenario, streamlining compliance workflows and saving time for your team.

To map DPIA questions to assessments,

* Select **Mappings** in the DPIA Questionnaire page.
* In the **Assessment Mappings** dialog, select your preferred question set for each assessment type.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/DPIA - Assessment Mappings.png" alt="" width="347"><figcaption></figcaption></figure></div>

Then, select **Save Mappings** to apply the configuration.

> * A single questionnaire set can be mapped to one, multiple, or all assessment types simultaneously.
> * If a field is left umppaed, the system automatically applies the pre-seeded Default DPIA risk question set.

<mark style="color:$warning;">**Queries/Suggestions**</mark><mark style="color:$warning;">:</mark>

* <mark style="color:$warning;">"Generate Risk questions with AI" option is not working.</mark>
* <mark style="color:$warning;">No instructions or templates are provided for uploading questions via XLSX or CSV once user begins adding sections manually.</mark>&#x20;
* <mark style="color:$warning;">Apart from the available assessment types, will there be any other assessment types? If so, how can we add them?</mark>

