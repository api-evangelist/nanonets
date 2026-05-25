# Nanonets (nanonets)
Nanonets is a no-code document AI and OCR platform. It combines a custom-model OCR API, pre-built document models (invoices, receipts, purchase orders, bills of lading, passports, driver's licenses, bank statements), image classification, and a visual workflow builder for imports, transformations, lookups, approvals, and ERP/CRM/database exports. The Nanonets OCR-3 model and the open-source `docext` toolkit power the IDP Leaderboard #1 ranking. The Enterprise tier adds SAML SSO, SCIM, role-based access, HIPAA, SOC 2 Type II, ISO 27001, on-prem and private-cloud deployment.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - AI, Artificial Intelligence, OCR, Document AI, Intelligent Document Processing, Data Extraction, Workflow Automation, Computer Vision, No-Code

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Nanonets OCR API
Synchronous and asynchronous OCR prediction and training over `app.nanonets.com/api/v2/OCR/Model/{model_id}`. Upload files by local path or public URL, retrieve predictions for a file, page, or batch, and train or retrain custom Nanonets OCR models. Sync endpoints are optimized for ≤3-page files; async endpoints handle larger documents. Returns labels, bounding boxes, OCR text, confidence scores, and table cell predictions.

**Human URL:** [https://docs.nanonets.com/reference/overview](https://docs.nanonets.com/reference/overview)

- [Documentation — Overview](https://docs.nanonets.com/reference/overview)
- [Documentation — Sync file prediction](https://docs.nanonets.com/reference/ocrmodellabelfilebymodelidpost-1)
- [Documentation — Async file prediction](https://docs.nanonets.com/reference/ocrmodellabelfileasyncbymodelidpost-1)
- [Documentation — Sync URL prediction](https://docs.nanonets.com/reference/ocrmodellabelurlsbymodelidpost)
- [Documentation — Async URL prediction](https://docs.nanonets.com/reference/ocrmodellabelurlsasyncbymodelidpost-1)
- [Documentation — Get prediction by file ID](https://docs.nanonets.com/reference/ocrmodelgetpredictionfilebyfileid)
- [Documentation — Get prediction by page ID](https://docs.nanonets.com/reference/ocrmodelgetpredictionfilebypageid)
- [Documentation — List prediction files](https://docs.nanonets.com/reference/ocrmodellistpredictionfiles)
- [Documentation — Upload training images by file](https://docs.nanonets.com/reference/ocrmodeluploadfilebymodelidpost-1)
- [Documentation — Upload training images by URL](https://docs.nanonets.com/reference/ocrmodeluploadurlsbymodelidpost-1)
- [Documentation — Train model](https://docs.nanonets.com/reference/ocrmodeltrainbymodelidpost-1)
- [OpenAPI](openapi/nanonets-ocr-api-openapi.yml)
- [JSON Schema — Prediction](json-schema/nanonets-prediction-schema.json)
- [JSON-LD](json-ld/nanonets-context.jsonld)
- [Naftiko Capability — OCR Prediction](capabilities/ocr-prediction.yaml)
- [Naftiko Capability — OCR Training](capabilities/ocr-training.yaml)
- [Example — Predict File](examples/nanonets-ocr-predict-file-example.json)

### Nanonets Image Classification API
Classify images by file upload or by publicly accessible URL against a Nanonets image classification model. Supports batch URL submission for efficient prediction.

**Human URL:** [https://docs.nanonets.com/reference/imagecategorizationlabelfilepost](https://docs.nanonets.com/reference/imagecategorizationlabelfilepost)

- [Documentation — Classify file](https://docs.nanonets.com/reference/imagecategorizationlabelfilepost)
- [Documentation — Classify URLs](https://docs.nanonets.com/reference/imagecategorizationlabelurlspost2)
- [OpenAPI](openapi/nanonets-image-classification-api-openapi.yml)
- [Naftiko Capability — Image Classification](capabilities/image-classification.yaml)
- [Example — Classify URLs](examples/nanonets-image-classify-urls-example.json)

### Nanonets File Management API
Approve, unapprove, assign, update, delete, and export files within a Nanonets model. Drives review-and-approval workflows, PATCH-based field updates, team assignment to specific reviewers, and export retry to downstream destinations.

**Human URL:** [https://docs.nanonets.com/reference/file-review-api](https://docs.nanonets.com/reference/file-review-api)

- [Documentation — File Review](https://docs.nanonets.com/reference/file-review-api)
- [Documentation — Assign Files](https://docs.nanonets.com/reference/assign-files-via-api)
- [Documentation — Update Fields](https://docs.nanonets.com/reference/update-fields-via-api)
- [Documentation — Delete Files](https://docs.nanonets.com/reference/delete-files-via-api)
- [Documentation — Export Files](https://docs.nanonets.com/reference/export-files-via-api)
- [OpenAPI](openapi/nanonets-file-management-api-openapi.yml)
- [Naftiko Capability — File Management](capabilities/file-management.yaml)

### Nanonets External Integrations API
List external integrations connected to a Nanonets account (PostgreSQL, MySQL, MSSQL, MongoDB) and execute generic SQL queries against them in the context of a workflow. Used by Database Matching Conditions and database lookup blocks.

**Human URL:** [https://docs.nanonets.com/reference/getexternalintegrations](https://docs.nanonets.com/reference/getexternalintegrations)

- [Documentation — Get External Integrations](https://docs.nanonets.com/reference/getexternalintegrations)
- [Documentation — Execute Query](https://docs.nanonets.com/reference/executequery-1)
- [OpenAPI](openapi/nanonets-external-integrations-api-openapi.yml)
- [Naftiko Capability — External Integrations](capabilities/external-integrations.yaml)

## Common Properties

- [Portal — nanonets.com](https://nanonets.com)
- [Console — app.nanonets.com](https://app.nanonets.com)
- [Documentation — docs.nanonets.com](https://docs.nanonets.com)
- [GettingStarted — Nanonets Overview](https://docs.nanonets.com/docs/nanonets-overview)
- [Authentication](https://docs.nanonets.com/reference/authentication)
- [Errors](https://docs.nanonets.com/reference/response-code-error)
- [RateLimits — Handle 429](https://docs.nanonets.com/reference/how-to-handle-429-error)
- [Documentation — Generate API Key](https://docs.nanonets.com/docs/generate-api-key)
- [Documentation — Async and Sync File Processing](https://docs.nanonets.com/docs/async-and-sync-file-processing)
- [Documentation — Supported File Formats](https://docs.nanonets.com/docs/file-formats)
- [Documentation — Languages Supported](https://docs.nanonets.com/docs/language-supported)
- [Webhooks — Webhook Export and Payload](https://docs.nanonets.com/docs/webhook-export)
- [Blog](https://nanonets.com/blog/)
- [SignUp](https://accounts.nanonets.com/signup)
- [TermsOfService](https://legal.nanonets.com/terms)
- [PrivacyPolicy](https://legal.nanonets.com/privacy)
- [Documentation — Data Processing Agreement](https://legal.nanonets.com/dpa)
- [GitHubOrganization — NanoNets](https://github.com/NanoNets)
- [Documentation — Postman Workspace](https://www.postman.com/nanonetsapi/nanonets)
- [Documentation — Hugging Face open models](https://huggingface.co/nanonets)
- [Documentation — IDP Leaderboard](https://www.idp-leaderboard.org/)
- [GitHubRepository — docext](https://github.com/NanoNets/docext)
- [GitHubRepository — docstrange](https://github.com/NanoNets/docstrange)
- [GitHubRepository — nanoindex](https://github.com/NanoNets/nanoindex)
- [SDK — Python (nanonets-python-client)](https://github.com/NanoNets/nanonets-python-client)
- [SDK — JavaScript / Node.js](https://github.com/NanoNets/nanonets-javascript)
- [SDK — Go](https://github.com/NanoNets/nanonets-go)
- [SDK — OCR Node.js SDK](https://github.com/NanoNets/ocr-js-sdk)
- [SDK — Image Classification Node.js SDK](https://github.com/NanoNets/ic-js-sdk)
- [CodeExamples — Object Detection (Python)](https://github.com/NanoNets/object-detection-sample-python)
- [CodeExamples — Object Detection (Node.js)](https://github.com/NanoNets/object-detection-sample-nodejs)
- [CodeExamples — Object Detection (Go)](https://github.com/NanoNets/object-detection-sample-golang)
- [CodeExamples — Object Detection (PHP)](https://github.com/NanoNets/object-detection-sample-php)
- [CodeExamples — OCR Python sample](https://github.com/NanoNets/nanonets-ocr-sample-python)
- [Tools — n8n nodes for Nanonets](https://github.com/NanoNets/n8n-nodes-nanonets)

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Nanonets OCR API](openapi/nanonets-ocr-api-openapi.yml)
- [Nanonets Image Classification API](openapi/nanonets-image-classification-api-openapi.yml)
- [Nanonets File Management API](openapi/nanonets-file-management-api-openapi.yml)
- [Nanonets External Integrations API](openapi/nanonets-external-integrations-api-openapi.yml)

### JSON Schema

- [Nanonets Prediction Schema](json-schema/nanonets-prediction-schema.json)

### JSON-LD

- [Nanonets Context](json-ld/nanonets-context.jsonld)

### Capabilities (Naftiko)

- [OCR Prediction](capabilities/ocr-prediction.yaml)
- [OCR Training](capabilities/ocr-training.yaml)
- [Image Classification](capabilities/image-classification.yaml)
- [File Management](capabilities/file-management.yaml)
- [External Integrations](capabilities/external-integrations.yaml)

### Vocabulary

- [Nanonets Vocabulary](vocabulary/nanonets-vocabulary.yml)

### Spectral Rules

- [Nanonets Spectral Ruleset](rules/nanonets-rules.yml)

### Examples

- [OCR — Predict File](examples/nanonets-ocr-predict-file-example.json)
- [Image Classification — Classify URLs](examples/nanonets-image-classify-urls-example.json)

### Commercial artifacts

- [Plans / Pricing](plans/nanonets-plans-pricing.yml)
- [Rate Limits](rate-limits/nanonets-rate-limits.yml)
- [FinOps Definition](finops/nanonets-finops.yml)

## Maintainers

**FN:** Kin Lane

**Email:** info@apievangelist.com
