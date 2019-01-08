| id |        Name        |                    Description                   |
|----|--------------------|--------------------------------------------------|
| 0  | InteractionId      | The unique ID for that session                   |
| 1  | UserId             | The unique ID of the end user.                   |
| 2  | State              | US State.                                        |
| 3  | UserAgentString    | The user agent string.                           |
| 4  | Browser            | The brand of web browser used.                   |
| 5  | BrowserVersion     | The version of web browser used.                 |
| 6  | DeviceIsMobile     | True if it was a mobile device; otherwise false. |
| 7  | DeviceBrand        | Brand of device (e.g. iPhone).                   |
| 8  | ScreenWidth        | The screen resolution width.                     |
| 9  | ScreenHeight       | The screen resolution height.                    |
| 10 | EventType          | The type of event that was logged                |
| 11 | Event              | The specific event that was logged               |
| 12 | RecordDateTime     | The timestamp of the event                       |

-----

Events in Quoting Process:
  1. Pre-Quote Portal
  2. Quote Start XOR Retrieve Existing Policy
  3. Retrieve Premium
  4. Bind Start
  5. Add Drivers
  6. Add Vehicles
  7. Choose Coverage
  8. Get Premium
  9. Payment Start
  10. Payment Complete
  11. Download Receipt

-----

From the perspective of events that are important to us,
  - Pre-Quote Portal is the landing page all customers begin at.
  - We define a quote as any user who makes it to the Retrieve Premium step.
  - We define a bind as any user who makes it to the Bind Start step.
  - We define a sale as any user who makes it to the Payment Complete step.

A "quote" is here defined as a user having completed our 3-minute quoting process widely advertised in our media campaigns. A "bind" event is defined as a user having submitted additional personal and demographic information (such as vehicles to insure, drivers, details about past accidents and violations). At that point, we are able to give users a more accurate quoted premium for their insurance policy. Lastly is when a user actually chooses to purchase their auto insurance policy from us.

Anything that occurs between these events is interesting to us, but less crucial. (For instance, it's interesting to spot users who generate multiple quotes in a short span of time. This might inidcate that they are trying to manipulate our online form to obtain a more favorable rate. But if they don't ever actually purchase a policy, this information becomes suddenly much less actionable for us.)
