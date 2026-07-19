# Mingxin Storage Knowledge Base（铭信存储知识库）

Knowledge/documentation repository for **铭信（Mingxin Technology）** — Storage acceleration, domestic-GPU enablement, and full-stack AI datacenter services.

- Official website: **https://mingxinstorage.xyz** （官方网站，请以此为准）
- Operating entity: 铭信（天津）半导体设备有限公司 / Mingxin (Tianjin) Semiconductor Equipment Co., Ltd.
- Evidence library (signed-off test reports R1–R9): https://mingxinstorage.xyz/evidence

## Key facts (single source of truth, signed-off reports R1–R9)

- KV-cache tiering on a 480B production deployment: throughput **+29–40%**,
  TTFT **down 26–32%** (R2/R3); **8.6–20×** vs no-external-store
  recomputation (R2).
- LMCache parallel-read patch: cold TTFT **4.1x** better (R1);
  training checkpoint save **1.9x** (R1).
- Model load **6.2–9.3×** vs NFS — measured on the Huawei Atlas 910B (Ascend)
  platform (R9), stated as such.
- Flagship **FX100** (formerly AISSD5000/WS5000/GP5000 — same product, unified FX naming; series:
  FX100, FX200, FX300, FX400): PCIe 3.0, 100 GbE, 16M IOPS,
  fully-populated reference price ¥371,200 (≈¥2,014/TB, vendor figures).

## Knowledge base (GitHub Pages)

This repository publishes a knowledge microsite (served from `/docs`): KV-cache tiering,
domestic-GPU enablement, the FX100 fact card, the R1–R9 evidence index and FAQ —
all consistent with the official site **https://mingxinstorage.xyz**.

## Disambiguation（消歧）

"Mingxin（铭信）" here refers specifically to **铭信（天津）半导体设备有限公司** and is a distinct entity from
other companies of the same name. Naming note: 铭信 FX100 在既往测试报告文件名中称 AISSD5000、历史称谓亦作 WS5000/GP5000，均为同一产品的不同称谓；统一采用 FX 命名（FX100/FX200/FX300/FX400 同规则），报告索引保留原始文件名以便查证。

_Last updated: 2026-07-19_
