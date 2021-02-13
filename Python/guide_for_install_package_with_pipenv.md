# Guide for install Package with Pipenv
---

**Pre-Install**
 1. เครื่องต้องติดตั้ง python, pip, pipenv ก่อน
	 - `python -m pip install`
	 - `pip install pipenv` 
 2. Create Folder Project

<br/>

**Setup Pipenv**
 1. พิมพ์คั่ง `pipenv install` 
 2. พิมพ์คำสั่ง `pipenvshell`
 3. สังเกตว่าจะมีไฟล์ pipfile, pipfile.lock ขึ้นมาในโปรเจคของเรา
 
<br/>


**Install Package**
1. cd เข้าไปใน folder project
2. พิมพ์คำสั่ง `pipenv shell`
3. ให้สั่งเกตที่หน้า cursor ของ teminal จะมี () ชื่อโปรเจคของเรา
4. พิมพ์คำสั่ง `pipenv install {packagename=version}`
5. เมื่อโหลดเสร็จแล้ว จะมีชื่อ Package Django ขึ้นมาในไฟล์ Pipfile
<br/>


**Uninstall Package**
1. cd เข้าไปใน folder project
2. พิมพ์คำสั่ง `pipenv shell`
3. พิมพ์คำสั่ง `pipenv uninstall {packagename=version}`
<br/>


**วิธีนำไปใช้งานกับเครื่องอื่น**
1. cd เข้าไปใน folder project
2. พิมพ์คำสั่ง `pipenv shell`
3. พิมพ์คำสั่ง `pipenv install`
4. ตัว pip จะไล่ติดตั้ง Package ที่ต้องใช้สำหรับโปจเจคเราโดยอัตโนมัติ
<br/>


> ***หากต้องการ ติดตั้ง Package อื่นเพิ่มเติม ก็ให้ทำเหมือนข้างต้น*** 
> ***อย่าลืม active shell ก่อนทุกครั้ง `pipenv shell`***


---


> __pipenv__
> > เป็นเครื่องมือ ที่ช่วยจัดการ python package dependency
> 
> > มีการสร้าง virtualenv ให้อัตโนมัติ (เรียกง่ายคือ tool ของ pip ที่รวมการสร้าง env และ package management ไว้ในตัวเดียว)
> 
> > ให้สนใจแค่ไฟล์ pipfile ถ้าเราต้องการเพิ่ม หรือ ปรับแต่งอะไร

<br/>

> __pipenv__
>> __Pipenv__ is a tool that aims to bring the best of all packaging worlds (bundler, composer, npm, cargo, yarn, etc.) to the Python world. Windows is a first-class citizen, in our world.
>>
>> It automatically creates and manages a virtualenv for your projects, as well as adds/removes packages from your Pipfile as you install/uninstall packages. It also generates the ever-important Pipfile.lock, which is used to produce deterministic builds.

