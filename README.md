
<div align="center">


# AIHawk: the first Jobs Applier AI Agent


AIHawk's core architecture remains **open source**, allowing developers to inspect and extend the codebase. However, due to copyright considerations, we have removed all third‑party provider plugins from this repository.

For a fully integrated experience, including managed provider connections: check out **[laboro.co](https://laboro.co/)** an AI‑driven job board where the agent **automatically applies to jobs** for you.


---


AIHawk has been featured by major media outlets for revolutionizing how job seekers interact with the job market:

[**Business Insider**](https://www.businessinsider.com/aihawk-applies-jobs-for-you-linkedin-risks-inaccuracies-mistakes-2024-11)
[**TechCrunch**](https://techcrunch.com/2024/10/10/a-reporter-used-ai-to-apply-to-2843-jobs/)
[**Semafor**](https://www.semafor.com/article/09/12/2024/linkedins-have-nots-and-have-bots)
[**Dev.by**](https://devby.io/news/ya-razoslal-rezume-na-2843-vakansii-po-17-v-chas-kak-ii-boty-vytesnyaut-ludei-iz-protsessa-naima.amp)
[**Wired**](https://www.wired.it/article/aihawk-come-automatizzare-ricerca-lavoro/)
[**The Verge**](https://www.theverge.com/2024/10/10/24266898/ai-is-enabling-job-seekers-to-think-like-spammers)
[**Vanity Fair**](https://www.vanityfair.it/article/intelligenza-artificiale-candidature-di-lavoro)
[**404 Media**](https://www.404media.co/i-applied-to-2-843-roles-the-rise-of-ai-powered-job-application-bots/)

</div>

## Setup

### Prerequisites
- Python 3.10 or newer
- [Google Chrome](https://www.google.com/chrome/) installed (used by Selenium)

### Installation
1. Clone the repository and move into it:
   ```bash
   git clone https://github.com/feder-cr/Jobs_Applier_AI_Agent_AIHawk.git
   cd Jobs_Applier_AI_Agent_AIHawk
   ```
2. (Optional but recommended) create and activate a virtual environment:
   ```bash
   python -m venv .venv
   source .venv/bin/activate   # On Windows use: .venv\Scripts\activate
   ```
3. Install Python dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Configuration
1. Copy the example data folder and update it with your information:
   ```bash
   cp -r data_folder_example data_folder
   ```
2. Edit the files inside `data_folder`:
   - `secrets.yaml` – add your LLM API key under `llm_api_key`.
   - `plain_text_resume.yaml` – fill in your resume details.
   - `work_preferences.yaml` – set your job search preferences.
   - Optionally adjust logging and model defaults in `config.py`.

### Running the agent
1. Start the application:
   ```bash
   python main.py
   ```
2. Follow the interactive prompts to build resumes and apply for jobs.
   Generated output is saved in `data_folder/output`.

