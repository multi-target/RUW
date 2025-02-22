# RUW
This repository provides a reference implementation of the paper:  
RUW: A Multi-Target Stance Detection Approach on the Russian-Ukrainian Issue  
which is under review.  
# Abstract
In this paper, we introduce RUW, an artificially annotated multi-target stance detection dataset. This dataset is set against the backdrop of the Russia-Ukraine conflict and is designed to analyze Twitter users' stances on both sides of the conflict during the Russia-Ukraine war. RUW is composed of 6,000 tweets collected through the Twitter API, with each tweet manually annotated as favor, against, or neutral toward each target. We explored the dataset by analyzing and modeling it using the Latent Dirichlet Allocation (LDA) model. We then conducted further analysis of our dataset using both machine learning and deep learning models to validate its feasibility. Additionally, we introduced a knowledge distillation model based on contrastive learning (KDCL). This model enables the effective learning of limited textual information through contrastive learning and knowledge distillation. We demonstrated the effectiveness of this approach on multiple datasets. We are making our new dataset publicly available to foster further research in multi-target stance detection.
# Environment settings
- python==3.7.4  
- numpy==1.21.6  
- pandas==1.3.5  
- tweet-preprocessor==0.6.0  
- scikit-learn==1.0.2
# Experimental results
The following table shows the results of several models run on both datasets.  

<table class=MsoTableGrid border=0 cellspacing=0 cellpadding=0
 style='border-collapse:collapse;border:none;mso-yfti-tbllook:1184;mso-padding-alt:
 0cm 5.4pt 0cm 5.4pt;mso-border-insideh:none;mso-border-insidev:none'>
 <tr style='mso-yfti-irow:0;mso-yfti-firstrow:yes'>
  <td width=105 rowspan=2 valign=top style='width:78.75pt;border-top:solid windowtext 1.0pt;
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;
  mso-border-top-alt:solid windowtext .5pt;mso-border-bottom-alt:solid windowtext .5pt;
  padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><a name="_Hlk143418719"><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>Model<o:p></o:p></span></a></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=264 colspan=3 valign=top style='width:197.75pt;border-top:solid windowtext 1.0pt;
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;
  mso-border-top-alt:solid windowtext .5pt;mso-border-bottom-alt:solid windowtext .5pt;
  padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;text-indent:22.0pt'><span
  style='mso-bookmark:_Hlk143418719'><span lang=EN-US style='font-size:11.0pt;
  mso-bidi-font-size:10.5pt'>2016 US election (%)<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=93 valign=top style='width:69.5pt;border:none;border-top:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal align=center style='text-align:center;text-indent:0cm;
  mso-char-indent-count:0'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>RUW (%)<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
 </tr>
 <tr style='mso-yfti-irow:1'>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=79 valign=top style='width:59.45pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-top-alt:solid windowtext .5pt;mso-border-top-alt:solid windowtext .5pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>Tr-Cl<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=92 valign=top style='width:69.15pt;border-top:solid windowtext 1.0pt;
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;
  mso-border-top-alt:solid windowtext .5pt;mso-border-bottom-alt:solid windowtext .5pt;
  padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>Tr-Cr<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=92 valign=top style='width:69.15pt;border-top:solid windowtext 1.0pt;
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;
  mso-border-top-alt:solid windowtext .5pt;mso-border-bottom-alt:solid windowtext .5pt;
  padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>Cl-Sa<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=93 valign=top style='width:69.5pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'><span
  style='mso-bookmark:_Hlk143418719'></span>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'><o:p>&nbsp;</o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
 </tr>
 <tr style='mso-yfti-irow:2'>
  <td width=105 valign=top style='width:78.75pt;border:none;mso-border-top-alt:
  solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>DT<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=79 valign=top style='width:59.45pt;border:none;mso-border-top-alt:
  solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>41.55<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=92 valign=top style='width:69.15pt;border:none;mso-border-top-alt:
  solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>33.46<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=92 valign=top style='width:69.15pt;border:none;mso-border-top-alt:
  solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>42.28<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=93 valign=top style='width:69.5pt;border:none;mso-border-top-alt:
  solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>37.83<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
 </tr>
 <tr style='mso-yfti-irow:3'>
  <td width=105 valign=top style='width:78.75pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>KNN<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=79 valign=top style='width:59.45pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>50.42<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=92 valign=top style='width:69.15pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:20.9pt;mso-char-indent-count:1.9'><span
  style='mso-bookmark:_Hlk143418719'><span lang=EN-US style='font-size:11.0pt;
  mso-bidi-font-size:10.5pt'>42.20<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=92 valign=top style='width:69.15pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>42.65<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=93 valign=top style='width:69.5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>39.29<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
 </tr>
 <tr style='mso-yfti-irow:4'>
  <td width=105 valign=top style='width:78.75pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>LSTM<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=79 valign=top style='width:59.45pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>43.48<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=92 valign=top style='width:69.15pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>42.92<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=92 valign=top style='width:69.15pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>43.27<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=93 valign=top style='width:69.5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>41.30<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
 </tr>
 <tr style='mso-yfti-irow:5'>
  <td width=105 valign=top style='width:78.75pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  class=SpellE><span lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:
  10.5pt'>BilSTM</span></span></span><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'><o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=79 valign=top style='width:59.45pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>45.01<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=92 valign=top style='width:69.15pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>45.09<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=92 valign=top style='width:69.15pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>41.99<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=93 valign=top style='width:69.5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>42.08<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
 </tr>
 <tr style='mso-yfti-irow:6'>
  <td width=105 valign=top style='width:78.75pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  class=SpellE><span lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:
  10.5pt'>BiCE</span></span></span><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'><o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=79 valign=top style='width:59.45pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>53.04<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=92 valign=top style='width:69.15pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>48.92<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=92 valign=top style='width:69.15pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>48.17<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=93 valign=top style='width:69.5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>49.99<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
 </tr>
 <tr style='mso-yfti-irow:7'>
  <td width=105 valign=top style='width:78.75pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>BERT<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=79 valign=top style='width:59.45pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>58.20<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=92 valign=top style='width:69.15pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>56.22<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=92 valign=top style='width:69.15pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>55.03<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=93 valign=top style='width:69.5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>54.13<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
 </tr>
 <tr style='mso-yfti-irow:8'>
  <td width=105 valign=top style='width:78.75pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>BERT-A<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=79 valign=top style='width:59.45pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>66.94<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=92 valign=top style='width:69.15pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>63.53<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=92 valign=top style='width:69.15pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>60.15<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=93 valign=top style='width:69.5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>56.40<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
 </tr>
 <tr style='mso-yfti-irow:9'>
  <td width=105 valign=top style='width:78.75pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>CKD<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=79 valign=top style='width:59.45pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>67.88<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=92 valign=top style='width:69.15pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>64.69<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=92 valign=top style='width:69.15pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>60.55<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=93 valign=top style='width:69.5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.0pt'><span style='mso-bookmark:_Hlk143418719'><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>58.74<o:p></o:p></span></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
 </tr>
 <tr style='mso-yfti-irow:10;mso-yfti-lastrow:yes'>
  <td width=105 valign=top style='width:78.75pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.1pt'><span style='mso-bookmark:_Hlk143418719'><b><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>KDCL<o:p></o:p></span></b></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=79 valign=top style='width:59.45pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.1pt'><span style='mso-bookmark:_Hlk143418719'><b><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>79.81<o:p></o:p></span></b></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=92 valign=top style='width:69.15pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.1pt'><span style='mso-bookmark:_Hlk143418719'><b><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>79.21<o:p></o:p></span></b></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=92 valign=top style='width:69.15pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.1pt'><span style='mso-bookmark:_Hlk143418719'><b><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>75.69<o:p></o:p></span></b></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
  <td width=93 valign=top style='width:69.5pt;border:none;border-bottom:solid windowtext 1.0pt;
  mso-border-bottom-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'>
  <p class=MsoNormal style='text-indent:22.1pt'><span style='mso-bookmark:_Hlk143418719'><b><span
  lang=EN-US style='font-size:11.0pt;mso-bidi-font-size:10.5pt'>78.21<o:p></o:p></span></b></span></p>
  </td>
  <span style='mso-bookmark:_Hlk143418719'></span>
 </tr>
</table>

# Basic usage
We provide one processed dataset:   
Ruw is used for the target stance detection task.
# Contact info
Please contact XXX at XXX with any questions.
