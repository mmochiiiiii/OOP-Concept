# Abstract Class

คลาสที่ไม่สามารถสร้างอินสแตนซ์หรือวัตถุจากมันได้โดยตรง และถูกออกแบบมาเพื่อให้คลาสอื่นสืบทอด (inherit) คุณสมบัติและพฤติกรรมจากมัน คลาสนามธรรมช่วยให้เราสามารถกำหนดแม่แบบ (blueprint) สำหรับคลาสอื่น ๆ ที่ต้องการตามได้ โดยที่ไม่สามารถสร้างวัตถุจากคลาสนี้ได้



**คุณสมบัติของคลาสนามธรรม:**

1. **ไม่สามารถสร้างวัตถุ**: เราไม่สามารถสร้างอินสแตนซ์จากคลาสนามธรรมได้
2. **การกำหนดเมธอดที่ต้องมี**: คลาสนามธรรมสามารถกำหนดเมธอดที่เป็นนามธรรม (abstract methods) ซึ่งต้องถูกเขียนใหม่ในคลาสที่สืบทอด
3. **การแชร์คุณสมบัติ**: ใช้เพื่อสร้างคลาสฐานสำหรับกลุ่มคลาสที่มีคุณสมบัติร่วมกัน
