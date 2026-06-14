# Interview Q&A — Arm Staff Firmware Developer in Test

---

## HR Introductory Call

---

### Q1: Tell me about yourself.

**A:** I'm a senior embedded software developer with 15 years of experience in SoC, DSP, MCU, and FPGA-based systems. My recent work focused on Xilinx SoC-based LiDAR systems — bare-metal and low-level firmware, real-time processing, communication protocols, device bring-up, validation tools, and cross-functional integration. I stay hands-on and care deeply about code quality and robustness.

---

### Q2: Why are you interested in this role at Arm?

**A:** This is not just a next step in my career — it's a big leap. I've spent 15 years building embedded systems, and this role at Arm is the kind of opportunity I've been working towards: low-level firmware development at the highest level, close to the hardware, in a company whose architecture literally powers the world. Working on autonomous driving firmware at Arm feels like arriving exactly where I should be.

---

### Q3: Why Arm specifically?

**A:** Arm is a well-known and highly trusted global company with real impact across the industry. For me, working at Arm means a once-in-a-lifetime chance to shape the future of technology and help create something the world has never seen before. I also relate strongly to Arm's 10x mindset — taking responsibility not just for my own part, but for the system as a whole.

---

### Q4: What does "Staff" level mean to you and how do you fit it?

**A:** Staff means being a strong individual contributor with broader technical influence — not just delivering features, but shaping technical direction, raising standards, mentoring others, and taking ownership of complex cross-cutting problems. I've done this throughout my career: I've driven architecture decisions, mentored junior engineers, and built tools and systems that teams relied on.

---

### Q5: What are your salary expectations?

**A:** I'm looking for a market-competitive package for the Munich area. Based on the posted range of €104,700 – €141,700, I would expect to be positioned in the upper part of that range given my 15 years of hands-on experience.

---

### Q6: What is your notice period / when can you start?

**A:** I can start immediately and I have the legal right to work in Germany.

---

### Q7: What are you looking for in your next role?

**A:** I'm looking for a role where I stay close to the hardware, work on technically challenging problems, contribute to high-quality firmware and validation, and be part of a company where the work has a broader impact beyond a single product.

---

### Q8: Do you have any questions for us?

**A:**
- What does success look like in this role during the first 6 months?
- What are the main technical challenges the team is working on right now?
- How is the team structured in Munich?

---

## Behavioral

---

### Q9: Tell me about a technically complex project you led or owned.

**A:** At Scantinel I owned the full firmware stack for a Xilinx SoC-based FMCW LiDAR system — from bare-metal bring-up to real-time DSP pipelines and host communication. The first major challenge was integration between PL and PS domains: DMA transfers, interrupt handling, and data pipelines all had to be deterministic — the LiDAR generates data at a fixed rate, and any timing slip means lost measurements. I designed the architecture around that constraint from day one.

The second challenge was longevity. The codebase had to work across multiple hardware revisions, stay maintainable for a growing team, and be properly documented. I introduced a layered architecture with clean hardware abstraction, established coding and documentation standards, and made sure new engineers could onboard without needing me to explain every module personally.

---

### Q10: Tell me about a time you failed or made a significant mistake.

**A:** Once I was building a validation tool for algorithm verification. I invested significant time making it clean, well-structured, and extensible — the kind of code I'd be proud of. I delivered a couple of days late. In the end, the tool was used exactly once.

That was a good lesson: I was optimizing for a future that never came. A quick script would have done the job just as well, on time, and nobody would have noticed the difference. Since then I consciously ask myself before diving deep — what is the actual lifetime of this thing, and am I building for today's problem or an imaginary tomorrow?

---
