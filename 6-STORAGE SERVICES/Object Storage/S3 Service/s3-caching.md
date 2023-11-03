
# S3-Performance
- Scales automatic
- 3500 Put/Copy/Post/Delete requests per second per prefix
- 5500 Get/Head requests per second per prefix
- A prefix is like the path to the object or object key
- No limit to the number of prefixes
- Scale performance by creating parallel prefixes. 10 prefixes implies 55000 Get/Head requests per second
- Caching is done by CloudFront. It's a fast CDN that caches S3 content in geographically distributed edge locations
- Elastic Cache for Redis can be used as well. It's an in-memory cache for structured data e.g Object metadata