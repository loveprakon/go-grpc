# go-grpc


grpc  มีรูปแบบการสื่อสารระหว่าง client กับ server 4 แบบ

1. Unary
    client request server response กลับไป
    
2. Client-side streaming 
    client ส่ง message ให้ server เป็น stream
   (เยอะๆหลายๆ message) server จะ response ครั้ง
   เดียวเมื่อ client หยุดส่ง message

3. Server-side streaming
   client ส่ง message ไปให้ server ส่ง stream กลับมา

4. Bidirectional streaming
    ส่ง stream ใส่กันทั้ง 2 ฝ่าย