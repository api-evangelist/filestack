# Filestack GraphQL Schema

## Overview

This conceptual GraphQL schema represents the Filestack file upload, transformation, storage, and CDN delivery API. Filestack provides file uploading, content detection, transformations (image, video, document), and CDN delivery through a REST API. This schema models those capabilities in GraphQL type definitions.

## Source

- API Reference: https://www.filestack.com/docs/api/
- Transformation API: https://www.filestack.com/docs/transformations/
- Storage API: https://www.filestack.com/docs/storage/
- CDN: https://www.filestack.com/docs/cdn/
- Webhooks: https://www.filestack.com/docs/api/webhooks/
- Security: https://www.filestack.com/docs/security/

## Schema Design Notes

The schema models Filestack's core capabilities:

1. **File Management** - uploading, retrieving, and managing files via handles
2. **Transformations** - image, video, and document transformation pipelines
3. **Storage** - multi-cloud storage backends (S3, GCS, Azure, Backblaze, Dropbox, Box)
4. **CDN Delivery** - content delivery network URL generation and configuration
5. **Security** - policy-based access control with signed URLs
6. **Multipart Upload** - chunked upload sessions for large files
7. **Webhooks** - event-driven notifications for file lifecycle events

## Types Summary

| Category | Types |
|---|---|
| File Core | File, FileDetails, FileStatus, FileName, FileSize, FileMimeType, FileURL, CDNUrl, Handle, FileHandle |
| Security | SecurityPolicy, SecuritySignature, PolicyOptions, APIKey, Token, Security |
| Transforms | Transform, TransformDetails, ImageTransform, DocumentTransform, VideoTransform |
| Image Ops | Resize, Crop, Rotate, Flip, Flop, Grayscale, Blur, Sharpen, Overlay, Watermark |
| Output | Format, AutoCompress, AutoFormat, Quality, Progressive |
| Download | Download, DownloadDetails |
| Storage | Store, StoreDetails, StorageProvider, S3Store, GCSStore, AzureStore, BackblazeStore, DropboxStore, BoxStore, StoreOptions |
| Upload | MultipartUpload, UploadChunk, UploadSession |
| CDN | CDN, CDNDetails |
| Transformation Pipeline | Transformation, TransformationDetails |
| Webhooks | Webhook, WebhookEvent |
| Configuration | PickerConfig, WorkerFunction |

## Schema File

See [filestack-schema.graphql](filestack-schema.graphql) for the full type definitions.
