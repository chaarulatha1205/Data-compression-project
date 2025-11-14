# Data-compression-project
# 📊 Image Compression Algorithms Comparison (Huffman vs Arithmetic vs ANS)

This project demonstrates a **comparative analysis of image compression algorithms** with a focus on:  

- **Huffman Coding**  
- **Arithmetic Coding**  
- **Asymmetric Numeral Systems (ANS)**  

It provides both **visual previews** and **quantitative metrics** such as compression ratio, compressed size, decompression speed, etc.  
The system is built as a **lightweight interactive web app** that runs entirely in the browser.  

---

## 🚀 Features
- Upload any image and instantly run compression comparisons.  
- Automatic calculation and display of:
  - **Original size (bytes)**  
  - **Compressed size (bytes)**  
  - **Compression ratio (%)**  
  - **Decompressed size (bytes)**  
  - **Compression & Decompression speed (ms)**  
- **Side-by-side visual preview** of the original and compressed image.  
- **Automatic highlight of best algorithm** (lowest compressed size).  
- Fully **responsive & interactive UI** (works on desktop and mobile).  

---

## 📊 Example Results

Here’s an example of compression results for a sample image:

| Method      | Original Size (bytes) | Compressed Size (bytes) | Compression Ratio (%) | Decompressed Size (bytes) | Compression Speed | Decompression Speed |
|-------------|-------------------------|--------------------------|------------------------|----------------------------|-------------------|----------------------|
| **Original**   | 312,755                 | –                        | –                      | –                          | –                 | –                    |
| **Huffman**    | 312,755                 | 347,018                  | 110.96% (worse)        | 312,755                    | Fastest (~10ms)   | Fastest (~8ms)       |
| **Arithmetic** | 312,755                 | 202,036                  | 64.60%                 | 312,755                    | Slow (~30–40ms)   | Slow (~25–30ms)      |
| **ANS**        | 312,755                 | 132,546                  | 42.38% ✅               | 312,755                    | Fast (~12ms)      | Fast (~10ms)         |

👉 **Observation:**  
- Huffman is fastest but doesn’t compress well.  
- Arithmetic gives better compression but is slower.  
- **ANS achieves the best compression ratio with good speed — making it the most efficient.**  

---

## 🖼️ UI Preview
*(Example screenshot of the comparison table)*  

<img width="940" height="427" alt="image" src="https://github.com/user-attachments/assets/42049d67-7c4f-4caf-9b5a-e28dd12a3095" />
After selecting the respective image :
<img width="940" height="455" alt="image" src="https://github.com/user-attachments/assets/a6bbb28b-ad5e-44e6-87f6-8e1081d380d9" />
When you click “Enter” , It opens a new page displaying the different compression types:
<img width="940" height="486" alt="image" src="https://github.com/user-attachments/assets/b7ce6b22-69a0-48a2-88c3-b723ee09121f" />
Now , The user can download the compressed file :
<img width="940" height="553" alt="image" src="https://github.com/user-attachments/assets/81d9ba24-2319-46c0-8e84-d0649603fc11" />
<img width="940" height="367" alt="image" src="https://github.com/user-attachments/assets/1003cab7-8eb0-4f54-9a4b-ed189c21d259" />


---

## 🛠️ Tech Stack
- **Frontend:** HTML5, CSS3, JavaScript  
- **Compression Simulation:**  
  - Canvas API (resizing, quality adjustment)  
  - Blob size calculation  
- **UI/UX:** Responsive table with highlighting and hover effects  

No external dependencies – runs directly in browser.  

---

## 📂 Project Structure
<img width="880" height="840" alt="image" src="https://github.com/user-attachments/assets/73923685-8d6d-4364-8ac1-7a1a1100c382" />
---

## 👩‍💻 Authors

- **Chaarulatha J**
- **Bharath Balaji S**
- **Adharsh Aravinth**
- **Yogalakshmi G**
- **Rahul J**

---

## 📜 License & Copyright

© 2025 Chaarulatha J, Bharath Balaji S, Adharsh Aravinth, Yogalakshmi G, Rahul J.  
All rights reserved.

This project is licensed for **educational and research purposes only**.  
Unauthorized commercial use, distribution, or modification is prohibited without prior permission from the authors.





