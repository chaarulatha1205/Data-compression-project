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

<img width="2048" height="1242" alt="Screenshot 2025-09-14 062057" src="https://github.com/user-attachments/assets/27029308-a645-4b14-b082-9b80340f1f33" />

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
📦 image-compression-comparison
 ┣ 📜 index.html          # Main web interface
 ┣ 📜 style.css           # Styling for UI
 ┣ 📜 script.js           # Orchestrates compression workflow
 ┣ 📂 algorithms/         # Compression algorithm implementations
 ┃ ┣ 📜 huffman.js        # Huffman Coding implementation
 ┃ ┣ 📜 arithmetic.js     # Arithmetic Coding implementation
 ┃ ┗ 📜 ans.js            # Asymmetric Numeral Systems implementation
 ┣ 📂 assets/
 ┃ ┗ 📜 sample.jpg        # Example test image
 ┣ 📂 docs/
 ┃ ┗ 📜 demo.png          # Screenshot for README
 ┗ 📜 README.md           # Documentation

# 📘 Compression Algorithms

This project demonstrates **three key entropy coding algorithms**: Huffman, Arithmetic, and ANS.  
Below are their **concepts, formulas, and pseudocode**.

---

## 1️⃣ Huffman Coding
**Concept:** Assign shorter binary codes to frequent symbols and longer codes to rare ones, forming a **prefix-free code**.

### 🔹 Formula
- **Entropy (lower bound of average length):**  
\[
H(X) = - \sum_{i=1}^{n} p(x_i) \log_2 p(x_i)
\]

- **Expected code length:**  
\[
L = \sum_{i=1}^{n} p(x_i) \cdot l(x_i)
\]  
where \(l(x_i)\) is the code length of symbol \(x_i\).

### 🔹 Pseudocode

