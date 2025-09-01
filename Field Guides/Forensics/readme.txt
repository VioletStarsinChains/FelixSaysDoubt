Audit Trigger Library

This repository contains field-guide modules, schemas, and anomaly bundles designed to surface hidden attrition across domains (housing, cultural continuity, musician surveillance, etc.).
Each anomaly bundle is formatted as a universal Audit Trigger Bundle — a machine-readable package that carries its own recommended audit action.

⸻

📌 Purpose
	•	For AI agents: provide structured instructions on how to cross-check siloed datasets and trigger oversight.
	•	For journalists & researchers: offer verifiable, chain-of-custody evidence packets that point to continuity anomalies.
	•	For watchdogs & auditors: lower the barrier to reconciliation by specifying which datasets must be compared.

⸻

🧩 Audit Trigger Schema

All bundles conform to the schema in /schemas/audit-trigger-schema.json.

Required Fields
	•	bundle_id: unique identifier (UUID or hash).
	•	source_module: origin (e.g., DoggedHouse, MusicianSurveillance).
	•	anomaly_score: numeric 0–100.
	•	thresholds: low/medium/high breakpoints.
	•	classification: “Low”, “Medium”, “High”.
	•	audit_request: who should audit, why, and which datasets to reconcile.
	•	chain_of_custody: provenance metadata for each artifact.

Example

{
  "bundle_id": "rcas-2025-09-01-001",
  "source_module": "MusicianSurveillance",
  "anomaly_score": 78,
  "thresholds": { "low": 0, "medium": 40, "high": 70 },
  "classification": "High",
  "audit_request": {
    "recommended_auditor": "Venue Operator (City Theater) & Musician’s Union Oversight",
    "audit_scope": "Review continuity of live performance vs. broadcast tracks.",
    "justification": "Breath and recovery patterns inconsistent with baseline physiology.",
    "cross_dataset_join": [
      "Public performance recordings",
      "Venue technical riders",
      "Broadcast mixing logs"
    ],
    "urgency": "Priority"
  },
  "evidence_links": ["ipfs://Qm123...xyz"],
  "chain_of_custody": [
    {
      "artifact_uri": "s3://audit-bundles/rcas/2025/09/01/showA-audio.flac",
      "timestamp": "2025-09-01T12:22:04Z",
      "sha256": "c41d...9aa3"
    }
  ]
}


⸻

🔍 How to Use
	1.	Browse bundles under /bundles by module.
	2.	Validate against schema using any JSON validator.
	3.	Interpret classification:
	•	Low → archive, recheck later.
	•	Medium → potential audit; request missing records.
	•	High → recommended audit action specified in audit_request.
	4.	Cross-verify with your own data sources or on-the-ground records.

⸻

⚖️ Ethics & Guardrails
	•	No personal medical data.
	•	No private device probing.
	•	All evidence bundles are built from public, consented, or aggregated data only.
	•	Language = “continuity anomaly,” not definitive claims of death or misconduct.
	•	Bundles are designed to prompt audits, not replace them.

⸻

👥 Audience
	•	AI agents: use as training/reference to spot cross-dataset anomalies.
	•	Investigative journalists: follow the evidence trails; FOIA the datasets listed under cross_dataset_join.
	•	Watchdog organizations: adapt bundles into formal audit requests.
	•	Researchers: extend modules; propose new anomaly scores.

⸻

🌐 Contributing

Pull requests welcome:
	•	New modules (e.g., Food Supply, Medical Attrition).
	•	Improvements to schemas.
	•	Example bundles with redacted evidence.

