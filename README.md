## LLM4BeSci_Bern2024

The course introduces the use of open-source large language models (LLMs) from the Hugging Face ecosystem for research in the behavioral.

By [Zak Hussain](https://zak-hussain.github.io/), [Rui Mata](https://matarui.org/research), and  [Dirk Wulff](https://www.mpib-berlin.mpg.de/person/93374/2549)

### Schedule

10:00 AM - 10:45 AM: Talk: Intro to LLMs <br>
10:45 AM - 11:00 AM: Break <br>
11:00 AM - 11:20 AM: Talk: A gentle to Python and Hugging Face <br>
11:20 AM - 12:00 AM: Exercises in Google Colab <br>
12:00 PM- 12:30 PM: Exercise Walkthrough and Q&A <br>

### Additional Resources
<a href="https://osf.io/preprints/psyarxiv/f7stn">Hussain, Binz, Mata, & Wulff (2024) A tutorial on open-source large language models for behavioral science
</a>
```@misc{hussain_binz_mata_wulff_2023,
 title={A tutorial on open-source large language models for behavioral science},
 url={osf.io/preprints/psyarxiv/f7stn},
 publisher={PsyArXiv},
 author={Hussain, Zak and Binz, Marcel and Mata, Rui and Wulff, Dirk U},
 year={2023},
 month={Dec},
 doi={https://doi.org/10.31234/osf.io/f7stn}
}
```

[Hugging face documentation](https://huggingface.co/docs)<br>
[Hugging face book](https://transformersbook.com/)<br>
[But what is a GPT (3Blue1Brown)](https://www.youtube.com/watch?v=wjZofJX0v4M&list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi&index=5)<br>

### Installation Instructions
0. If you do not have a Google account, you will need to create one (this can be deleted after the workshop).
1. Navigate to Google Drive (https://drive.google.com/).
2. In the top-left, click New > More > Colaboratory. If you do not see Colaboratory, you may need to click "Connect more apps", 
search for 'Colaboratory', and install it. Then click New > More > Colaboratory.
3. Copy the following code snipped into the first cell of the notebook. Run it (```shift + enter``` or click &#9658; button) to mount your Google Drive to the Colab environment.
A pop-up will ask you to connect; click through the steps to connect your Google Drive to Colab (you will have to do this
every time you open a new notebook).
```
from google.colab import drive
drive.mount("/content/drive")
```
4. Create a second cell in your notebook using the "+ Code" button that appears when you hover your cursor right under the first cell. Copy and run the following code snippet in the second cell of your notebook to clone the GitHub repository to your Google Drive :
```
%cd /content/drive/MyDrive
!git clone https://github.com/Zak-Hussain/LLM4BeSci_Bern2024.git
```
5. Go back to your Google Drive and navigate to the folder "LLM4BeSci_StGalen2024". You should see the relevant notebook (`exercises.ipynb`) and data files (it may take  a couple of minutes for the files to appear).

#### Hugging Face API Setup Instructions
The following steps are required to access the Llama-3 model via the Hugging Face API, which we will use in the workshop.

6. Make sure you have a Hugging Face account (https://huggingface.co/join) (it's free!). 
7. Go to the [Llama-3 model page](https://huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct) and fill in the 'META LLAMA 3 COMMUNITY LICENSE AGREEMENT' form at the top of the page in order to get access to the model (this can take up to an hour). 
8. Once you have been granted access, you can navigate to [your Hugging Face profile settings](https://huggingface.co/settings/tokens) to generate an API access token. Click 'New token' at the bottom of the page, give your token a name, and select  'Type'='Read'. This token should provide access to all models in the Llama family. 
9. If you wish to run the largest (70B parameter) version of Llama-3, you will need to have a Hugging Face PRO subscription (currently $9/month). You can also run the smaller versions (as in this notebook) with your free account.
