# Invoice Sentry Dashboard

A Streamlit-based dashboard to automate the request process for missing invoices and track their arrival.

## Features

- **Trip-based Grouping**: View invoices grouped by Trip Number with expandable sections
- **Individual Requests**: Send invoice requests to individual vendors with one click
- **Bulk Actions**: Request all missing invoices for an entire trip at once
- **Visual Feedback**: See which requests have been sent with clear status indicators
- **Email Preview**: Preview the email template before sending
- **Days Overdue Tracking**: Color-coded indicators for invoice urgency
- **Summary Statistics**: Overview of total trips, vendors, amounts, and sent requests

## Installation

1. Install the required dependencies:
```bash
pip install -r requirements.txt
```

2. Run the Streamlit app:
```bash
streamlit run app.py
```

The app will open in your default web browser at `http://localhost:8501`

## Usage

1. **View Trips**: Expand any trip section to see all vendors for that trip
2. **Send Individual Requests**: Click "📤 Send Request" on any vendor row
3. **Bulk Requests**: Click "📧 Request All Missing Invoices for this Trip" at the top of any expanded trip
4. **Preview Emails**: Click "👁️ Preview" to see the email template that will be sent
5. **Track Status**: Monitor which requests have been sent using the status indicators

## Data Structure

The dashboard displays:
- **Trip ID**: Unique identifier for each trip
- **Vendor Name**: Name of the vendor
- **Vendor Email**: Email address for invoice requests
- **Amount**: Invoice amount in dollars
- **Days Overdue**: Number of days the invoice is overdue (color-coded)

## Next Steps

The current implementation includes placeholder logic for sending requests. The next step is to integrate actual email sending functionality.

