# تحليل انطباعات الرأي العام ومعالجة اللغة الطبيعية في البيانات النصية

**إعداد:** أحمد نور الدين محمد  
**المؤهل والتخصص:** طالب محاسبة (السنة الثالثة)، معهد القاهرة الجديدة العالي | متدرب سابق في تحليل البيانات بالبنك التجاري الدولي (CIB)  
**البريد الإلكتروني:** ahmedn4474@gmail.com | **المستودع:** [https://github.com/ahmedn4474-art/Twitter-Sentiment-Classification](https://github.com/ahmedn4474-art/Twitter-Sentiment-Classification)  
**المجال التخصصي:** Natural Language Processing (NLP), Sentiment Mining & Text Analytics  
**البيانات المستخدمة:** Sentiment140 Corpus (Sampled 50,000 balanced benchmark records & Full 1.6M pipeline)  

---

## 1. ملخص تنفيذي وصياغة المشكلة

تولد شبكات التواصل الاجتماعي تدفقات ضخمة من النصوص والآراء اليومية. يطبق هذا المشروع مسارا لمعالجة اللغات الطبيعية (NLP) يشمل تنظيف النصوص واستخراج الخصائص عبر TF-IDF ونمذجة التصنيف السريع باستخدام الانحدار اللوجستي.

---

## 2. هيكل المشروع والملفات

`	ext
|-- data/                    # مجلد البيانات
|-- Twitter_Sentiment_Notebook.ipynb   # دفتر Jupyter Notebook مكتمل المخرجات والرسومات
|-- requirements.txt         # متطلبات وحزم بايثون
|-- README.md                # التقرير الفني باللغة الإنجليزية
|-- README_AR.md             # التقرير الفني باللغة العربية
`

---

## 3. كيفية تشغيل المشروع محليا

1. **نسخ المستودع (Clone):**
   `ash
   git clone https://github.com/ahmedn4474-art/Twitter-Sentiment-Classification.git
   cd Project2_Twitter_Sentiment
   `

2. **تثبيت الحزم المطلوبة:**
   `ash
   pip install -r requirements.txt
   `

3. **فتح دفتر العمل:**
   `ash
   jupyter notebook Twitter_Sentiment_Notebook.ipynb
   `

---

*إعداد: أحمد نور الدين محمد — تحليلات البيانات المالية والكمية.*
