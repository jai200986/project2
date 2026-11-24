# VIBRANCE 2026 - College Cultural Event Website Template

An energetic, modern, responsive college cultural event website built strictly using **HTML and CSS only (Zero JavaScript)**.

Designed specifically for collegiate fests, cultural carnivals, battle of the bands, dance crew showdowns, theatrical plays, and star night concerts. Fully fluid and mobile-responsive across phones, tablets, laptops, and ultra-wide desktop monitors.

---

## 📁 Project Structure

```text
PROJECT/
├── index.html        # Complete semantic HTML5 structure with placeholders
├── style.css         # Modern pure CSS stylesheet with design tokens & variables
└── README.md         # Customization guide and instructions (this file)
```

---

## ✨ Features Included

1. **Pure CSS Responsive Navigation**:
   - Sticky header with glassmorphism blur effect (`backdrop-filter`).
   - Accessible pure CSS mobile hamburger drawer menu using the checkbox-hack (`#nav-toggle:checked ~ .main-navigation`), featuring animated "hamburger" to "X" transformation.
   - Smooth anchor scrolling (`scroll-behavior: smooth`) with header offset padding.

2. **Hero Section**:
   - High-energy collegiate branding with glowing neon radial orbs.
   - Event Title, Theme pill, Tagline, and quick Date &amp; Time keycard.
   - Live pure CSS Countdown Display cards (Days, Hours, Minutes, Seconds).
   - High-impact statistics ribbon (Competitions, Footfall, Cash Prizes, Star Nights).

3. **About the Fest**:
   - Festival legacy, 2026 Theme spotlight (*"Ignite the Spectrum"*).
   - 4 Core Pillars of the Fest (Acoustics & Stage, National Credibility, Festival Food Village, Inclusive Community).

4. **Event Categories & Competitions (45+ Events)**:
   - 6 category cards:
     - 🎸 **Music & Bands** (Battle of the Bands, Eastern Harmony, Rap Cypher, Acoustic Unplugged)
     - 💃 **Dance Extravaganza** (Western Crew, 1v1 Street Cyphers, Classical Solo)
     - 👗 **Fashion & Runway** (Thematic Couture, Mr. &amp; Ms. Vibrance)
     - 🎭 **Theatre & Drama** (National Nukkad Natak, Proscenium One-Act, Mime)
     - 🎨 **Fine Arts & Media** (Graffiti Murals, 24-Hr Film Race, Photography)
     - 🎮 **E-Sports & Gaming** (Valorant LAN, EA FC / FIFA 25, BGMI, Cosplay)
   - Meta tags for stages, prize money badges, team sizes, and direct registration links.

5. **Interactive 3-Day Schedule Timetable (Pure CSS Tabs)**:
   - Seamlessly switch between **Day 1 (Friday)**, **Day 2 (Saturday)**, and **Day 3 (Sunday)** using pure CSS radio buttons without page reloads.
   - Hour-by-hour program slots with venue badges, category tags, and highlighted **Star Night** concert slots.

6. **Star Performers & Celebrity Guests**:
   - Headline EDM Producer / DJ Act (Day 3 Grand Finale).
   - National Indie-Rock Band (Day 1 Opener).
   - Celebrity Stand-Up Comedian (Day 2 Special Act).
   - Chief Dance Jury & Masterclass Mentor.

7. **Venue & Campus Layout**:
   - Official College Address, GPS Coordinates, and Campus Status pill.
   - Campus Zone guide (Zones A, B, C, D, E).
   - Pure CSS Illustrated Campus Schematic with gates, main arena, amphitheater, auditorium, food court, and parking.
   - Direct link to open in Google Maps / Apple Maps.

8. **Travel, Transit & Accommodation Guide**:
   - Directions by **Metro / Subway**, **City Bus & Shuttles**, **Railway Station**, and **Personal Vehicles & Parking**.
   - Outstation Student Accommodation banner with subsidized hostel charges and direct hospitality helplines.

9. **Festival Passes & Ticket Tiers**:
   - **Student General Pass** (Free with valid College ID)
   - **Competitor All-Access Pass** (Highlighted as Most Popular)
   - **VIP Star Night Pass** (Front-row concert pit & artist meet-and-greet)

10. **Comprehensive Student Registration Form**:
    - Fields: Full Name, Email, Phone/WhatsApp, College Name, Roll No. / Student ID, Year of Study, Pass Type, Competition Category, Team Name & Size, Special Requests/Stay Notes, and Code of Conduct checkbox.
    - **Pure CSS Confirmation Modal**: On submit, the form triggers `#reg-success:target`, displaying a stylish confirmation pass badge and next-step instructions.

11. **Frequently Asked Questions (FAQ)**:
    - Native HTML5 `<details>` and `<summary>` accordions with animated `+` to `×` rotation.

12. **Sponsors & Complete Footer**:
    - Title, Powered By, Beverage, Audio, and Media partner slots.
    - Emergency medical helpline, Registration desk numbers, Dean/Convener contacts, and social media handles.

---

## 🎨 How to Customize Content & Details

All placeholder items in `index.html` are explicitly marked with bracketed tags like `[PLACEHOLDER]` so you can easily find and replace them using your code editor's Find and Replace (`Ctrl + H` or `Cmd + H`).

### 1. Change College and Event Name
Open `index.html` and search for:
- `[APEX INSTITUTE OF TECHNOLOGY]` or `[COLLEGE NAME]` &rarr; Replace with your institution's name (e.g. *St. Xavier's College*, *IIT Bombay*, *BITS Pilani*).
- `VIBRANCE 2026` or `[COLLEGE FEST NAME]` &rarr; Replace with your fest name (e.g. *OASIS 2026*, *MOOD INDIGO*, *MILAN 2026*).

### 2. Update Festival Dates & Timings
- In `index.html`, search for `April 17 – 19, 2026` and replace with your exact dates.
- Search for `9:00 AM – 10:30 PM` and update daily operating timings.
- In the **Countdown Section** (`line 144`), update the static numbers (`48 Days`, `14 Hours`, etc.) to match your festival countdown.

### 3. Update the Festival Theme
- Find `"IGNITE THE SPECTRUM"` and replace with your festival theme (e.g. *"Retro-Futurism: Neon Echoes"*, *"Chronicles of Tomorrow"*, *"Kaleidoscope: Colors of Chaos"*).

### 4. Customize the Schedule
- Navigate to the `<section class="schedule-section" id="schedule">` in `index.html`.
- Each day's events are organized under:
  - `.panel-day1` (Day 1)
  - `.panel-day2` (Day 2)
  - `.panel-day3` (Day 3)
- Simply edit the event titles, times (`<span class="time-main">`), venues, and descriptions.

### 5. Replace Performers and Celebrities
- Search for `performer-card` in `index.html`.
- Replace placeholder names like `[DJ KRONOS]`, `[THE NEON ECHOES]`, and `[AARAV MEHTA]` with your confirmed celebrity artists, along with their performance times and stages.
- Replace image URLs in `src="..."` with your artist's promotional photos.

### 6. Adjust Campus Address & Travel Information
- Search for `[Apex Main Campus]` and update the address, gate numbers, nearest metro station name, and bus routes.
- Replace `https://maps.google.com` in the map card with your college's specific Google Maps location link.

### 7. Customizing the Color Palette via CSS Variables
Open `style.css` and customize the variables in `:root` (lines 12–45):

```css
:root {
  /* Change brand colors here */
  --color-primary: #8b5cf6;       /* Main neon accent (violet) */
  --color-accent: #f43f5e;        /* Secondary accent / CTA color (rose) */
  --color-cyan: #06b6d4;          /* Cyber cyan details */
  --color-amber: #f59e0b;         /* Gold star badges */

  /* Dark Canvas Colors */
  --color-bg-base: #0a0b12;       /* Base background */
  --color-bg-card: rgba(22, 27, 49, 0.75); /* Card surface */
}
```

---

## 📱 Responsiveness Testing

The template is fully responsive and tested for:
- **Mobile Phones (320px – 480px)**: Compact single-column view, touch-friendly buttons, full-screen mobile menu drawer.
- **Tablets (600px – 1024px)**: 2-column grids for events, performers, and contact information.
- **Laptops & Desktops (1024px – 1920px)**: Full multi-column grid, horizontal navigation bar, interactive schematic map.

---

## 🚀 How to View the Website

Double-click `index.html` to open it directly in any modern web browser (Google Chrome, Mozilla Firefox, Microsoft Edge, Safari, or Opera). No local web server or build tool is required!
