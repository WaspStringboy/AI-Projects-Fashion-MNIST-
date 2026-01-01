# 這個專案將引導初學者透過使用 TensorFlow 框架，對 Fashion MNIST 數據集進行圖像識別的深度學習模型的設計、開發和評估，並且可以試著將模型下載分享與視覺化模型架構。從基礎理論到實務操作，本專案旨在為初學者逐步了解深度學習的過程，並且帶領讀者從數據預處理到模型訓練和評估，進而掌握如何在實際情境中應用深度學習模型。<br/>


# 1. 學習目標<br/>
1.瞭解深度學習(Deep Learning)和神經網路(Neural Networks)的基本概念。<br/>
2.掌握使用 TensorFlow 進行進行數據處理、模型建構、訓練和評估的技巧。<br/>
3.學會進行數據正規化和模型參數的調整。<br/>
4.實作建構、訓練和評估深度學習模型。<br/>
5.提升問題解決和模型優化的能力。<br/>

# 2. 步驟說明<br/>
# Step 1. 數據載入及預處理# Ste
載入數據集：使用 TensorFlow 的 Keras API 載入 Fashion MNIST 數據集，這是一個常提供給初學者使用的深度學習圖像分類數據集。是由 60,000 個圖像的訓練集(training set)和 10,000 個圖像的測試集(test set)所組成。每個圖像都是一個 28×28 灰階影像，與 10 個類別的標籤相關聯。<br/>
import tensorflow as tf<br/>

mnist = tf.keras.datasets.fashion_mnist<br/>

(training_images, training_labels), (test_images, test_labels) = mnist.load_data()<br/>

# Step 2. 顯示第一個訓練圖像<br/>
備註：本步驟提供想學習查看訓練資料圖像內容的讀者參考，若不需要則可以考慮跳至下一個步驟，不會影響本專案學習。<br/>

導入 matplotlib 函式庫來顯示圖像<br/>
import matplotlib.pyplot as plt<br/>
顯示第一個訓練圖像<br/>
plt.imshow(training_images[0])<br/>
![image](1.png)<br/>









