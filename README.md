<img src = "https://raw.githubusercontent.com/Faris4166/Simple-Checklist-Application-in-Python/refs/heads/main/BG.jpg">

# 🌟 โปรแกรมแสดงลวดลายพีระมิดดาว (Star Pyramid) ด้วย Python

---

## 📋 รายละเอียดโปรแกรม

โปรแกรมนี้เป็นโปรแกรมง่าย ๆ ที่ใช้ภาษา Python สร้างลวดลายรูปพีระมิด โดยใช้เครื่องหมายดาว `*` แสดงผลบนหน้าจอคอมพิวเตอร์

โปรแกรมจะถามผู้ใช้ว่าต้องการให้พีระมิดมีกี่แถว จากนั้นก็จะแสดงลวดลายดาวตามจำนวนแถวนั้น โดยให้ดาวเรียงตัวเป็นรูปสามเหลี่ยมที่กึ่งกลางหน้าจอ

---

## 🧑‍🏫 อธิบายหลักการทำงาน (แบบคนทั่วไป)

### 1. รับข้อมูลจำนวนแถว

- โปรแกรมจะถามว่า "ต้องการให้พีระมิดมีจำนวนกี่แถว?"  
- เราก็พิมพ์ตัวเลขลงไป เช่น 5 แล้วกด Enter

### 2. วาดพีระมิดทีละแถว

- โปรแกรมจะเริ่มวาดจากแถวบนสุดไปล่างสุดทีละแถว
- แต่ละแถวจะมีช่องว่าง (พื้นที่ว่าง) ขึ้นอยู่กับแถว เพื่อให้ดาวอยู่ตรงกลาง
- แล้วก็จะพิมพ์ดาวจำนวนหนึ่งในแถวนั้น (แถวบนสุดดาวน้อยสุด แถวล่างสุดดาวมากสุด)

### 3. การจัดวางดาว

- ช่องว่างด้านซ้ายจะลดลงทุกแถว ทำให้ดาวกว้างขึ้นไปทางขวา
- จำนวนดาวในแต่ละแถวเป็นเลขคี่ เช่น 1, 3, 5, 7... เพื่อให้รูปทรงสมมาตรสวยงาม

### 4. ขึ้นบรรทัดใหม่

- เมื่อวาดดาวครบแถวหนึ่ง โปรแกรมจะขึ้นบรรทัดใหม่เพื่อวาดแถวถัดไป

---

## 💻 โค้ดโปรแกรมตัวอย่าง

```python
rows = int(input("Enter number of rows: "))  # รับจำนวนแถวจากผู้ใช้

for i in range(rows):                         # วนลูปตามจำนวนแถว
    for j in range(rows - i - 1):             # วนพิมพ์ช่องว่างด้านหน้าแถว
        print(" ", end="")                    # พิมพ์ช่องว่างโดยไม่ขึ้นบรรทัดใหม่
    for j in range(2 * i + 1):                # วนพิมพ์ดาวจำนวน (2*i + 1) ดวง
        print("*", end="")                    # พิมพ์ดาวโดยไม่ขึ้นบรรทัดใหม่
    print()                                  # ขึ้นบรรทัดใหม่หลังจบแต่ละแถว
```

---
<div align="center">
  <img src="https://i.pinimg.com/originals/b7/76/78/b776782000fd19e82c2cd63c069cd298.gif" alt="centered gif">
</div>

