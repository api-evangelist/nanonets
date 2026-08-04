# Nanonets (nanonets)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Nanonets is a no-code document AI and OCR platform that combines a custom-model OCR API, pre-built document models (invoices, receipts, purchase orders, bills of lading, passports, driver's licenses, bank statements), image classification, and a visual workflow builder with imports, transformations, lookups, approvals, and ERP/CRM/database exports. The Nanonets OCR-3 model and the open-source docext toolkit power the IDP Leaderboard number-one ranking. Enterprise tier adds SAML SSO, SCIM, role-based access, on-prem and private-cloud deployment, HIPAA, SOC 2 Type II, and ISO 27001.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/apis.yml)

## Scope

- **Access:** 3rd-Party

## Tags

- AI
- Artificial Intelligence
- OCR
- Document AI
- Intelligent Document Processing
- Data Extraction
- Workflow Automation
- Computer Vision
- No-Code

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Nanonets OCR API

Synchronous and asynchronous OCR prediction and training endpoints over `app.nanonets.com/api/v2/OCR/Model/{model_id}`. Upload files by local path or public URL, retrieve predictions for a file, page, or batch, and train or retrain custom Nanonets OCR models. Sync endpoints are optimized for files of 3 pages or fewer; async endpoints handle larger documents. Returns labels, bounding boxes, OCR text, confidence scores, and table cell predictions.

- **Human URL:** [https://docs.nanonets.com/reference/overview](https://docs.nanonets.com/reference/overview)

#### Tags

- OCR
- Document AI
- Data Extraction
- Intelligent Document Processing

#### Properties

- [Documentation](https://docs.nanonets.com/reference/overview)
- [Documentation](https://docs.nanonets.com/reference/ocrmodellabelfilebymodelidpost-1)
- [Documentation](https://docs.nanonets.com/reference/ocrmodellabelfileasyncbymodelidpost-1)
- [Documentation](https://docs.nanonets.com/reference/ocrmodellabelurlsbymodelidpost)
- [Documentation](https://docs.nanonets.com/reference/ocrmodellabelurlsasyncbymodelidpost-1)
- [Documentation](https://docs.nanonets.com/reference/ocrmodelgetpredictionfilebyfileid)
- [Documentation](https://docs.nanonets.com/reference/ocrmodelgetpredictionfilebypageid)
- [Documentation](https://docs.nanonets.com/reference/ocrmodellistpredictionfiles)
- [Documentation](https://docs.nanonets.com/reference/ocrmodeluploadfilebymodelidpost-1)
- [Documentation](https://docs.nanonets.com/reference/ocrmodeluploadurlsbymodelidpost-1)
- [Documentation](https://docs.nanonets.com/reference/ocrmodeltrainbymodelidpost-1)
- [OpenAPI](openapi/nanonets-ocr-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/nanonets-ocr-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/nanonets-ocr-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/nanonets-prediction-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/nanonets-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Nanonets Image Classification API

Classify images by file upload or by publicly accessible URL against a Nanonets image classification model. Supports batch URL submission for efficient prediction. Base path `/api/v2/ImageCategorization/LabelFile/` and `/api/v2/ImageCategorization/LabelUrls/`.

- **Human URL:** [https://docs.nanonets.com/reference/imagecategorizationlabelfilepost](https://docs.nanonets.com/reference/imagecategorizationlabelfilepost)

#### Tags

- Image Classification
- Computer Vision
- Deep Learning

#### Properties

- [Documentation](https://docs.nanonets.com/reference/imagecategorizationlabelfilepost)
- [Documentation](https://docs.nanonets.com/reference/imagecategorizationlabelurlspost2)
- [OpenAPI](openapi/nanonets-image-classification-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/nanonets-image-classification-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/nanonets-image-classification-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Nanonets File Management API

Approve, unapprove, assign, update, delete, and export files within a Nanonets model. Drives the review-and-approval workflow, PATCH-based field updates, team assignment to specific reviewers, and export retry to downstream destinations (Salesforce, QuickBooks, Xero, Google Sheets, SAP, etc.).

- **Human URL:** [https://docs.nanonets.com/reference/file-review-api](https://docs.nanonets.com/reference/file-review-api)

#### Tags

- File Management
- Workflow
- Approvals
- Documents

#### Properties

- [Documentation](https://docs.nanonets.com/reference/file-review-api)
- [Documentation](https://docs.nanonets.com/reference/assign-files-via-api)
- [Documentation](https://docs.nanonets.com/reference/delete-files-via-api)
- [Documentation](https://docs.nanonets.com/reference/export-files-via-api)
- [Documentation](https://docs.nanonets.com/reference/update-fields-via-api)
- [Documentation](https://docs.nanonets.com/docs/retry-file-upload-via-api)
- [OpenAPI](openapi/nanonets-file-management-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/nanonets-file-management-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/nanonets-file-management-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Nanonets External Integrations API

List external integrations connected to a Nanonets account (Postgres, MySQL, MSSQL, MongoDB, and other databases) and execute generic SQL queries against them in the context of a Nanonets workflow. Used by Database Matching Conditions and database lookup actions inside the no-code workflow builder.

- **Human URL:** [https://docs.nanonets.com/reference/getexternalintegrations](https://docs.nanonets.com/reference/getexternalintegrations)

#### Tags

- Integrations
- Database
- Lookups

#### Properties

- [Documentation](https://docs.nanonets.com/reference/getexternalintegrations)
- [Documentation](https://docs.nanonets.com/reference/executequery-1)
- [OpenAPI](openapi/nanonets-external-integrations-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/nanonets-external-integrations-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/nanonets-external-integrations-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Portal](https://nanonets.com)
- [Console](https://app.nanonets.com)
- [Documentation](https://docs.nanonets.com)
- [Getting Started](https://docs.nanonets.com/docs/nanonets-overview)
- [Authentication](https://docs.nanonets.com/reference/authentication)
- [Errors](https://docs.nanonets.com/reference/response-code-error)
- [Rate Limits](https://docs.nanonets.com/reference/how-to-handle-429-error)
- [Documentation](https://docs.nanonets.com/docs/generate-api-key)
- [Documentation](https://docs.nanonets.com/docs/async-and-sync-file-processing)
- [Documentation](https://docs.nanonets.com/docs/file-formats)
- [Documentation](https://docs.nanonets.com/docs/language-supported)
- [Webhooks](https://docs.nanonets.com/docs/webhook-export)
- [Blog](https://nanonets.com/blog/)
- [Sign Up](https://accounts.nanonets.com/signup)
- [Terms of Service](https://legal.nanonets.com/terms)
- [Privacy Policy](https://legal.nanonets.com/privacy)
- [Documentation](https://legal.nanonets.com/dpa)
- [GitHub Organization](https://github.com/NanoNets)
- [Documentation](https://www.postman.com/nanonetsapi/nanonets)
- [Documentation](https://huggingface.co/nanonets)
- [Documentation](https://www.idp-leaderboard.org/)
- [GitHub Repository](https://github.com/NanoNets/docext)
- [GitHub Repository](https://github.com/NanoNets/docstrange)
- [GitHub Repository](https://github.com/NanoNets/nanoindex)
- [SDK](https://github.com/NanoNets/nanonets-python-client)
- [SDK](https://github.com/NanoNets/nanonets-javascript)
- [SDK](https://github.com/NanoNets/nanonets-go)
- [SDK](https://github.com/NanoNets/ocr-js-sdk)
- [SDK](https://github.com/NanoNets/ic-js-sdk)
- [Code Examples](https://github.com/NanoNets/object-detection-sample-python)
- [Code Examples](https://github.com/NanoNets/object-detection-sample-nodejs)
- [Code Examples](https://github.com/NanoNets/object-detection-sample-golang)
- [Code Examples](https://github.com/NanoNets/object-detection-sample-php)
- [Code Examples](https://github.com/NanoNets/nanonets-ocr-sample-python)
- [Tools](https://github.com/NanoNets/n8n-nodes-nanonets)
- [Plans](plans/nanonets-plans-pricing.yml)
- [Rate Limits](rate-limits/nanonets-rate-limits.yml)
- [Fin Ops](finops/nanonets-finops.yml)
- [Spectral Rules](rules/nanonets-rules.yml)
- [Vocabulary](vocabulary/nanonets-vocabulary.yml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
