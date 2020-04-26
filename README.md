# YOLOv3 ile Kendi Nesne Tanıma Modelini Geliştirme
<p><a target="_blank" rel="noopener noreferrer" href="https://github.com/emrecintas/Yolov3_Kendi_Nesne_Tanima_Modelini_Gelistirme/blob/master/iha.png"><img src="https://github.com/emrecintas/Yolov3_Kendi_Nesne_Tanima_Modelini_Gelistirme/blob/master/iha.png" alt="" style="max-width:100%;"></a></p>

Özel bir YOLOv3 dedektörü oluşturmak için aşağıdakilere ihtiyacımız olacak:

*   Etiketli Özel Veri Seti
*   Özel .cfg dosyası
*   obj.data ve obj.names dosyaları
*   train.txt dosyası (test.txt burada isteğe bağlıdır)

# 1. Adım: Özel Veri Kümesini Toplama ve Etiketleme

Özel bir nesne dedektörü oluşturmak için iyi bir görüntü ve etiket veri setine ihtiyacınız vardır, böylece dedektör nesneleri algılamak için verimli bir şekilde eğitilebilir.

Bu iki şekilde yapılabilir. [Google resimlerini kullanarak](https://storage.googleapis.com/openimages/web/index.html) veya kendi veri kümenizi oluşturarak ve etiketleri manuel olarak çizmek için bir ek açıklama aracını kullanarak. (İlk yolu tavsiye ederim! ilk yol için internetten araştırma ile google'dan özel veri seti indirebilirsiniz)

İkinci yol ile [labelimg vb kullanarak](https://tzutalin.github.io/labelImg/) resimleri etiketlemeniz ve resim dosyaları ile txt dosyalarını aynı isim olacak şekilde bir dosyada tutmanız gerekmektedir. (Emre.jpg - Emre.txt)

DETAYLAR;
<p><g-emoji class="g-emoji" alias="pushpin" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f4cc.png">📌</g-emoji>1 <a href="https://colab.research.google.com/github/emrecintas/Yolov3_Kendi_Nesne_Tanima_Modelini_Gelistirme/blob/master/Yolov3_Kendi_Nesne_Tanima_Modelini_Gelistirme.ipynb" rel="nofollow"><img src="https://camo.githubusercontent.com/52feade06f2fecbf006889a904d221e6a730c194/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667" alt="Open In Colab" data-canonical-src="https://colab.research.google.com/assets/colab-badge.svg" style="max-width:100%;"></a> <strong>Google Colab Not Defteri</strong></p>

<p><g-emoji class="g-emoji" alias="pushpin" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f4cc.png">📌</g-emoji>1 <a href="https://github.com/emrecintas/Yolov3_Kendi_Nesne_Tanima_Modelini_Gelistirme/blob/master/Yolov3_Kendi_Nesne_Tanima_Modelini_Gelistirme.ipynb" rel="nofollow"><img src="https://github.com/jupyter/notebook/raw/master/docs/resources/icon_32x32.svg?sanitize=true" alt="Open In Jupyter" style="max-width:100%;"></a> <strong>Jupyter Not Defteri</strong></p>
