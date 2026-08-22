# Tigris (tigris-data)

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Tigris is a globally distributed, multi-cloud, S3-compatible object storage service. Data is automatically placed close to where it is read for low latency worldwide, with no egress fees. The storage API speaks the AWS S3 protocol at https://t3.storage.dev (formerly fly.storage.tigris.dev) so existing boto3, AWS SDK, and S3 clients work unchanged, with companion IAM and CloudFront-compatible APIs for access keys and public-key signing.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/tigris-data/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/tigris-data/refs/heads/main/apis.yml)

## Tags

- Object Storage
- S3 Compatible
- Storage
- Multi-Cloud
- Globally Distributed

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### Tigris Object Storage (S3-Compatible) API

AWS S3-compatible object operations - PutObject, GetObject, HeadObject, CopyObject, DeleteObject, DeleteObjects, ListObjectsV2, object tagging, ranged and conditional reads, and storage-class tiering - served at https://t3.storage.dev and authenticated with AWS Signature Version 4.

- **Human URL:** [https://www.tigrisdata.com/docs/api/s3/](https://www.tigrisdata.com/docs/api/s3/)
- **Base URL:** `https://t3.storage.dev`

#### Tags

- Object Storage
- S3 Compatible
- Objects

#### Properties

- [Documentation](https://www.tigrisdata.com/docs/objects/)
- [API Reference](https://www.tigrisdata.com/docs/api/s3/)
- [OpenAPI](openapi/tigris-data-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tigris-data.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tigris-data.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Tigris Bucket Management API

S3-compatible bucket lifecycle and configuration - CreateBucket, ListBuckets, HeadBucket, DeleteBucket, plus CORS, lifecycle, tagging, ownership controls, notification configuration, and ACL settings on Tigris buckets.

- **Human URL:** [https://www.tigrisdata.com/docs/buckets/](https://www.tigrisdata.com/docs/buckets/)
- **Base URL:** `https://t3.storage.dev`

#### Tags

- Buckets
- S3 Compatible
- Management

#### Properties

- [Documentation](https://www.tigrisdata.com/docs/buckets/)
- [API Reference](https://www.tigrisdata.com/docs/api/s3/)
- [OpenAPI](openapi/tigris-data-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tigris-data.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tigris-data.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Tigris Multipart Upload API

S3-compatible multipart upload flow for large objects - CreateMultipartUpload, UploadPart, UploadPartCopy, ListParts, ListMultipartUploads, CompleteMultipartUpload, and AbortMultipartUpload.

- **Human URL:** [https://www.tigrisdata.com/docs/objects/](https://www.tigrisdata.com/docs/objects/)
- **Base URL:** `https://t3.storage.dev`

#### Tags

- Multipart
- Uploads
- Large Objects

#### Properties

- [Documentation](https://www.tigrisdata.com/docs/objects/)
- [API Reference](https://www.tigrisdata.com/docs/api/s3/)
- [OpenAPI](openapi/tigris-data-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tigris-data.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tigris-data.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Tigris Presigned URLs API

SigV4 presigned URLs for time-limited, credential-free object access - PresignGetObject, PresignPutObject, PresignHeadObject, PresignDeleteObject, and PresignUploadPart.

- **Human URL:** [https://www.tigrisdata.com/docs/objects/presigned-urls/](https://www.tigrisdata.com/docs/objects/presigned-urls/)
- **Base URL:** `https://t3.storage.dev`

#### Tags

- Presigned URLs
- Temporary Access
- S3 Compatible

#### Properties

- [Documentation](https://www.tigrisdata.com/docs/objects/presigned-urls/)
- [API Reference](https://www.tigrisdata.com/docs/api/s3/)
- [OpenAPI](openapi/tigris-data-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tigris-data.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tigris-data.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Tigris IAM and Access Keys API

AWS IAM-compatible API served at https://iam.storage.dev for managing access keys and policies - CreateAccessKey, ListAccessKeys, UpdateAccessKey, DeleteAccessKey, CreatePolicy, GetPolicy, ListPolicies, DeletePolicy, AttachUserPolicy, DetachUserPolicy, and ListUserPolicies. Tigris IAM uses policies attached directly to access keys rather than IAM users, groups, or roles.

- **Human URL:** [https://www.tigrisdata.com/docs/iam/](https://www.tigrisdata.com/docs/iam/)
- **Base URL:** `https://iam.storage.dev`

#### Tags

- IAM
- Access Keys
- Policies

#### Properties

- [Documentation](https://www.tigrisdata.com/docs/iam/)
- [API Reference](https://www.tigrisdata.com/docs/api/s3/)
- [OpenAPI](openapi/tigris-data-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tigris-data.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tigris-data.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Tigris Object Tiering API

Storage-class tiering using S3-compatible classes - STANDARD, STANDARD_IA (Infrequent Access), GLACIER (Archive), and GLACIER_IR (Archive Instant Retrieval) - set per bucket default or per object via the x-amz-storage-class header, with RestoreObject to restore archived objects.

- **Human URL:** [https://www.tigrisdata.com/docs/objects/tiers/](https://www.tigrisdata.com/docs/objects/tiers/)
- **Base URL:** `https://t3.storage.dev`

#### Tags

- Storage Tiers
- Lifecycle
- Cost Optimization

#### Properties

- [Documentation](https://www.tigrisdata.com/docs/objects/tiers/)
- [API Reference](https://www.tigrisdata.com/docs/api/s3/)
- [OpenAPI](openapi/tigris-data-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tigris-data.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tigris-data.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/tigrisdata)
- [LinkedIn](https://www.linkedin.com/company/tigrisdata)
- [Website](https://www.tigrisdata.com)
- [Documentation](https://www.tigrisdata.com/docs/)
- [Plans](plans/tigris-data-plans-pricing.yml)
- [Rate Limits](rate-limits/tigris-data-rate-limits.yml)
- [Fin Ops](finops/tigris-data-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
