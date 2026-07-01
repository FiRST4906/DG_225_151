```mermaid
mindmap
  root((Pac-Man))
    Theme
      เขาวงกต
      อาเขตยุค 80
    Mechanics
      เดินในเขาวงกต
      กิน Pellet
      Power Pellet
    Content
      ผีศัตรู 4 ตัว
      ผลไม้โบนัส
    Audience
      ผู้เล่น Casual
    Art Style
       Pixel
       สีสันสดใส
```

```mermaid
quadrantChart
 title Pac-Man — Feature Prioritization
 x-axis Low Effort --> High Effort
 y-axis Low Impact --> High Impact

 quadrant-1 Quick Wins
 quadrant-2 Major
 quadrant-3 Nice to Have
 quadrant-4 Reconsider

    Maze Movement: [0.2, 0.95]
    Ghost AI: [0.7, 0.9]
    Score System: [0.3, 0.8]
    Sound Effects: [0.4, 0.6]
    Pause Menu: [0.2, 0.4]
    Online Leaderboard: [0.9, 0.4]
    Character Skins: [0.8, 0.3]
```

ซ้ายบน Quick Wins → ควรอยู่ใน MVP ก่อน

ขวาบน Major Projects → อาจอยู่ใน MVP ได้ถ้าจำเป็นต่อระบบหลัก แต่ส่วนใหญ่ทำต่อจาก MVP

ขวาล่าง Nice to Have → ควรตัดออกก่อนหรือเลื่อนไปทำภายหลัง

ซ้ายล่าง Reconsider → พิจารณาว่าคุ้มค่าที่จะทำหรือไม่ เพราะแม้ทำง่ายแต่ให้ประโยชน์น้อย


```mermaid
gantt
    title Pac-Man - Production Timeline (6 สัปดาห์)
    dateFormat YYYY-MM-DD

    section Pre-Production
    Concept & GDD :done, c1, 2026-07-06, 5d

    section Production
    Maze Movement :active, p1, after c1, 5d
    Ghost AI :p2, after p1, 7d
    Pellet & Score :p3, after p2, 5d
    Pause Menu :p4, after p3, 3d

    section Milestone
    Alpha Build :milestone, a1, after p2, 0d

    section Post
    QA & Bug Fix :q1, after p4, 5d
    Release Build :milestone, r1, after q1, 0d
```
