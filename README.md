# Assignment 1

For **commit** "hello ninjas" code, here is the screenshot:
<img width="1710" height="1112" alt="Screenshot 2026-03-09 at 10 35 12" src="https://github.com/user-attachments/assets/f6e2dd52-2fe0-43af-95cf-95e60ab21b90" />
<img width="530" height="974" alt="Screenshot 2026-03-09 at 10 57 21" src="https://github.com/user-attachments/assets/696b0dcb-927e-40d6-a89f-a82c88587626" />

For **commit** "final code reference" code, here is the screenshot:
<img width="1710" height="1112" alt="Screenshot 2026-03-09 at 10 36 24" src="https://github.com/user-attachments/assets/1a243982-ea87-429f-a2dc-d95c9cd05895" />
<img width="551" height="971" alt="Screenshot 2026-03-09 at 10 55 18" src="https://github.com/user-attachments/assets/2b0f86be-ab4b-4a0b-b4f6-2a4677ce4d3a" />

# Assignment 2

## Widget Explanation (main.dart)

<img width="507" height="973" alt="Screenshot 2026-03-10 at 11 34 15" src="https://github.com/user-attachments/assets/5ddeeed6-908f-45a2-850a-6fcf9271cdbd" />

### Custom Widgets

#### 1. **MyApp** (StatelessWidget)
- **Purpose**: Root widget of the application
- **Type**: StatelessWidget (immutable, doesn't maintain state)
- **Key Properties**:
  - Returns a `MaterialApp` widget
  - Sets up the app theme with deep purple color scheme
  - Uses Material 3 design
  - Sets `RowColumnPage` as the home page

#### 2. **RowColumnPage** (StatelessWidget)
- **Purpose**: Main page displaying the UI layout with image, text, icons, and counter
- **Type**: StatelessWidget
- **Features**:
  - Uses `MediaQuery` to get screen dimensions
  - Returns a `Scaffold` with AppBar and body
  - Arranges children in a `Column` layout
  - Contains an image display section, text description, icon row, and counter card

#### 3. **CounterCard** (StatefulWidget)
- **Purpose**: Interactive counter widget that increments when button is pressed
- **Type**: StatefulWidget (maintains mutable state)
- **State Management**:
  - `_counter`: Integer variable that tracks the count
  - `_incrementCounter()`: Method that updates state using `setState()`
- **Features**:
  - Displays current counter value
  - Has an add button with `IconButton` that increments the counter

---

### Flutter Built-in Widgets Used

#### **MaterialApp**
- Root widget for Material Design apps
- Provides theme configuration, navigation, and routing
- Properties used: `title`, `theme`, `home`

#### **Scaffold**
- Provides basic material design visual structure
- Contains AppBar, body, and other components
- Used as the main page structure

#### **AppBar**
- Top app bar displaying the title "My First App"
- Properties: `title`, `backgroundColor`, `centerTitle`

#### **Column**
- Arranges children widgets vertically
- Properties used:
  - `crossAxisAlignment`: Center alignment horizontally
  - `mainAxisAlignment`: Center alignment vertically
  - `children`: List of child widgets

#### **Row**
- Arranges children widgets horizontally
- Properties used:
  - `mainAxisAlignment`: SpaceEvenly distribution
  - `crossAxisAlignment`: Start alignment
  - `children`: List of icon-text columns

#### **Container**
- Box widget for styling and positioning
- Properties used:
  - `margin`: Outer spacing with `EdgeInsets.fromLTRB()`
  - `padding`: Inner spacing with `EdgeInsets.all()`
  - `color`: Background color
  - `width`: Container width using `MediaQuery`
  - `child`: Single child widget

#### **AspectRatio**
- Maintains a specific aspect ratio (1:1 in this case)
- Used to create a square container for the image

#### **Image.network**
- Displays an image from the internet
- Properties:
  - `fit`: BoxFit.cover (fills the container)
  - `width`: Image width (500)
  - URL: 'https://picsum.photos/200'

#### **Text**
- Displays text strings
- Properties:
  - `style`: TextStyle to customize font size, color, etc.
- Used for labels and counter display

#### **Icon**
- Displays Material Design icons
- Icons used:
  - `Icons.food_bank`: Food icon
  - `Icons.landscape`: Scenery icon
  - `Icons.people`: People icon
  - `Icons.add`: Plus icon for counter button

#### **IconButton**
- Interactive button with an icon
- Properties:
  - `onPressed`: Callback function triggered on tap
  - `icon`: Icon widget to display

#### **MediaQuery**
- Provides screen size and device information
- Used with `.of(context).size.width` to make responsive layouts

#### **Center**
- Centers its child widget
- Used to center the network image
