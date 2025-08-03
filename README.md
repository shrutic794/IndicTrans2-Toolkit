# IndicTrans2-Toolkit

#  IndicTrans2 Translation Pipeline

End-to-end English ↔ Indic translation using [AI4Bharat/IndicTrans2](https://github.com/AI4Bharat/IndicTrans2), with support for BLEU, ROUGE, and METEOR evaluation.

---

##  Setup

```bash
git clone https://github.com/AI4Bharat/IndicTrans2.git
cd IndicTrans2/huggingface_interface
pip install nltk sacremoses pandas regex mock "transformers>=4.33.2" mosestokenizer
pip install bitsandbytes scipy accelerate datasets sentencepiece sacrebleu rouge-score
python -c "import nltk; nltk.download('punkt'); nltk.download('wordnet')"

git clone https://github.com/VarunGumma/IndicTransTokenizer
cd IndicTransTokenizer
pip install --editable ./

Features
Translate between English and 20+ Indic languages
Supports 4-bit/8-bit quantization for low-resource devices
Evaluation using BLEU, ROUGE, METEOR
Batch translation with GPU acceleration

👤 Credits
Built using:

AI4Bharat/IndicTrans2

VarunGumma/IndicTransTokenizer
