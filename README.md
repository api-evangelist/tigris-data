# Tigris (tigris-data)

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
