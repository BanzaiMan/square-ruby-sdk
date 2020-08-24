## Invoice Payment Reminder

Describes a payment request reminder (automatic notification) that Square sends
to the customer. You configure a reminder relative to the payment request
`due_date`.

### Structure

`InvoicePaymentReminder`

### Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `uid` | `String` | Optional | A Square-assigned ID that uniquely identifies the reminder within the<br>`InvoicePaymentRequest`. |
| `relative_scheduled_days` | `Integer` | Optional | The number of days before (a negative number) or after (a positive number)<br>the payment request `due_date` when the reminder is sent. For example, -3 indicates that<br>the reminder should be sent 3 days before the payment request `due_date`. |
| `message` | `String` | Optional | The reminder message. |
| `status` | [`String (Invoice Payment Reminder Status)`](/doc/models/invoice-payment-reminder-status.md) | Optional | The status of a payment request reminder. |
| `sent_at` | `String` | Optional | If sent, the timestamp when the reminder was sent, in RFC 3339 format. |

### Example (as JSON)

```json
{
  "uid": null,
  "relative_scheduled_days": null,
  "message": null,
  "status": null,
  "sent_at": null
}
```
