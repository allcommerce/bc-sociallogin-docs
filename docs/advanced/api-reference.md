# API Reference

## API Overview

Papa Social Login provides REST API for advanced integration and automation.

## Authentication

### API Keys
```bash
Authorization: Bearer YOUR_API_KEY
```

### Rate Limits
- **7-day trial**: Full API access
- **Standard plan**: 50,000 requests/month  
- **Higher limits**: Available on request

## Endpoints

### Customer Management
```bash
GET /api/v1/customers
POST /api/v1/customers
PUT /api/v1/customers/{id}
DELETE /api/v1/customers/{id}
```

### Social Profiles
```bash
GET /api/v1/customers/{id}/social-profiles
POST /api/v1/customers/{id}/link-social
DELETE /api/v1/customers/{id}/unlink-social
```

### Analytics
```bash
GET /api/v1/analytics/login-stats
GET /api/v1/analytics/conversion-metrics
```

## Webhooks

### Available Events
- `customer.social_login`
- `customer.account_created`
- `customer.profile_updated`

### Webhook Configuration
```json
{
  "url": "https://yourstore.com/webhooks/papa-social",
  "events": ["customer.social_login"],
  "secret": "webhook_secret_key"
}
```

## SDKs

### JavaScript SDK
```javascript
import PapaSocialLogin from '@papa/social-login-sdk';

const papa = new PapaSocialLogin({
  apiKey: 'your-api-key',
  storeHash: 'your-store-hash'
});
```

### PHP SDK
```php
use Papa\SocialLogin\Client;

$client = new Client([
    'api_key' => 'your-api-key',
    'store_hash' => 'your-store-hash'
]);
```

!!! info "API Documentation"
    Full API documentation available at [api-docs.papasociallogin.com](https://api-docs.papasociallogin.com)