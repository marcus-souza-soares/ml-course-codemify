# Hotel Booking Demand — Dataset Description

This dataset contains real booking records from two hotels in Portugal: a **city hotel** and a
**resort hotel**, with arrivals between July 2015 and August 2017. Each row is one booking. The
data includes when the booking was made, length of stay, guest counts, room and deposit details,
and whether the booking was ultimately canceled. All personally identifying information has been
removed from the data.

The prediction target for this project is **`is_canceled`**: whether the booking was canceled
(1) or not (0).

## Columns

| Column | Description |
|---|---|
| `hotel` | City Hotel or Resort Hotel |
| `is_canceled` | 1 if the booking was canceled, 0 otherwise (the target) |
| `lead_time` | Days between the booking date and the arrival date |
| `arrival_date_year` | Year of the arrival date |
| `arrival_date_month` | Month of the arrival date (name) |
| `arrival_date_week_number` | Week number of the arrival date |
| `arrival_date_day_of_month` | Day of the month of the arrival date |
| `stays_in_weekend_nights` | Weekend nights (Saturday/Sunday) booked |
| `stays_in_week_nights` | Week nights (Monday–Friday) booked |
| `adults` | Number of adults |
| `children` | Number of children |
| `babies` | Number of babies |
| `meal` | Meal package: BB (bed & breakfast), HB (half board), FB (full board), SC/Undefined (no meal) |
| `country` | Country of origin (3-letter ISO country code; a small number of entries use other formats) |
| `market_segment` | Booking segment, e.g. Online TA, Offline TA/TO, Groups, Direct, Corporate (TA = travel agent, TO = tour operator) |
| `distribution_channel` | Booking channel: TA/TO, Direct, Corporate, GDS, Undefined |
| `is_repeated_guest` | 1 if the booking was made by a repeated guest |
| `previous_cancellations` | Prior bookings canceled by this customer |
| `previous_bookings_not_canceled` | Prior bookings by this customer that were not canceled |
| `reserved_room_type` | Room type reserved (anonymized code) |
| `assigned_room_type` | Room type actually assigned (may differ from reserved) |
| `booking_changes` | Number of changes made to the booking |
| `deposit_type` | No Deposit, Non Refund, or Refundable |
| `agent` | ID of the travel agency that made the booking (anonymized) |
| `company` | ID of the company that made or paid for the booking (anonymized) |
| `days_in_waiting_list` | Days the booking waited before confirmation |
| `customer_type` | Contract, Group, Transient, or Transient-Party |
| `adr` | Average daily rate (total lodging revenue divided by staying nights) |
| `required_car_parking_spaces` | Parking spaces requested |
| `total_of_special_requests` | Number of special requests made |
| `reservation_status` | Last reservation status: Canceled, Check-Out, or No-Show |
| `reservation_status_date` | Date when the last status was set |

## Source & Acknowledgements

The data originates from the open-access research article:

> Nuno Antonio, Ana de Almeida, Luis Nunes, **"Hotel booking demand datasets"**,
> *Data in Brief*, Volume 22, February 2019, pages 41–49.
> https://doi.org/10.1016/j.dib.2018.11.126

The combined dataset was downloaded and cleaned by Thomas Mock and Antoine Bichat for
**#TidyTuesday** (week of February 11th, 2020), and is published on Kaggle as
[Hotel booking demand](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand).

**License:** [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
The file distributed with this course has been modified from the original for course use.
