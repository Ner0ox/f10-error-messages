# Error messages for the BMW F10 Cluster

# Usage

> [!NOTE]
> On byte 4 `0x29` (in our case), sends the alert to the cluster, and `0x28` clears it, specified by the `ERROR_CODE_HERE`

```
void sendAlerts() {
    unsigned char message[] = { 0x40, ERROR_CODE_HERE, 0x00, 0x29, 0xFF, 0xFF, 0xFF, 0xFF };
    CAN.sendMsgBuf(0x5c0, 0, 8, message);
}
```

# Codes
```
10 Chassis
11 Chassis
12, 13 cornering ability restricted
14, 15, 16, 17, door open
18 all doors open + hood
19,20  all doors + hood + trunk
21 ignition do not stop engine
22, 23 starter. do not stop engine
24 Brake system. Drive Moderately
25 Preheating. Please wait.
26 Cruise Control Failure!
27 Refill engine oil level
28 Engine oil low, please Refill
29 Drivetrain. Drive Moderately
30 Engine! Stop carefully
31 Increased Emissions!
32 Filler cap open!
33 Engine fault! Drive Moderately.
34 Check Engine light
35 DSC
36 DSC OFF
37 Trigger
38 DSC Deactivated
39 Engine overheated. Stop carefully
40 To start engine, press brake pedal
41 Service due
42 Brake system. Drive Moderately
43,44,45,46,47 cornering ability restricted
48 Red handbrake
50, 51 Flat Tyre Monitor (RPA) Failure
52 Protect against rolling away
53 Automatic Hold. Apply the brakes
54 Parking brake only partially available
55, 56 Release parking brake
57 Auto hold
58,59 Auto hold + green parking brake
60, 61 Instument cluster
62 Speed warning
63,64,65, Tyre pressure loss!
66 Remote control. No engine start
67 Remote control. Replace battery
68 Remote control for car parked functions
69 Cruise control. Keep your distance
70 Steering. Drive Moderately
71, 72, 73 Have the brake pads checked!
74 Brake system. Stop carefully
75 Trailer tow bar electrics
76 Trailer tow bar electrics
77 Trailer tow bar electrics
78 Speed warning
79 Outside temperature
80 Outside temperature
81 nothing
82 nothing
83 nothing
84 nothing
85 Active cruise control Deactivated
86 ^^
87 rear light right failure!
88 dipped beam left failure
89 dipped beam right failure
90 trailer reversing light failure
91 fasten seat belt
92 fasten seat belt
93 fasten seat belt
94 restraint system rear
95 restraint system rear right fault
96 restraint system rear right fault
97 restraint system
98 restraint system
99 restraint system
100 restraint system
101 restraint system
102 nothing
103 transmission too hot
104 transmission temp! drive Moderately
105 transmission temp! stop carefully
106 transmission temp! Stop carefully
107 ?
108 Driver restraint system
109 Passanger restraint system
110 Passanger restraint system
111 Passanger + Driver restraint system
112 Passanger + Driver restraint system
113 parking lights on
114 ?
115 reversing light failure
116 turn indicator left failure
117 left reversing light failure
118 rear light right failure
119 turn indicator right failure
120 dipped beam left failure
121 dipped beam right failure
122 turn indicator left failure
123 rear light left failure
124 rear light left failure
125 right rear turn indicator failure
126 fog light failure
127 fog light failure
128 high beam head light left failure
129 fog light at rear right failure
130 high beam headlight right failure
131 parking /daytime light failure
132 parking light front right failure
133 rear light left failure
134 brake light right failure
135 Brake light right failure
136 Brake light left failure
137 Brake light left failure
138 fog light failure
139 tyre pressure low stop carefully
140 tyre pressure low stop carefully
141 tyre pressure low stop carefully
142 check tyre pressure. initialise rdc?
143 tyre pressure low stop carefully
144 RDC fault. drive Moderately
145 tyre press. control Deactivated
146 tyre press control Deactivated
147 tyre pressure low. stop carefully
148 tyre pressure low. stop carefully
149 RDC failure. drive Moderately
150 armoured luggage-compt door open
151 gas alarm! air system on
152 disconnect charging cable!
153 gun mount fault
154 irritant gas sensor fault
155  irritant gas sensor fault
156 air system not functioning
157 air system active
158 air system active
159 doors not locked
160 use window lifter emergency system
161 second battery defect
162 strobe light. check bulb
163 fire exting active
164 washer fluid level low
165 outside temperature
166 top up the coolant
167 top up coolant
168 nothing
169 gearbox in N only with engine on!
170 transmission fault
171 transmission fault
172 transmission fault
173 transmission drive Moderately
174 gearbox in position P only at standstill!
175 secure vehicle against rolling
176 Active Cruise control failure!
177 active cruise control failure
178 active cruise control failure
179 transmission drive Moderately
180 driving comfort restricted
181 driving comfort restricted
182 transmission drive Moderately
183 windscreen wiper
184 dynamic tractio ncontrol activated
185 gear selector-lever indicator
186 steerng wheel lock defective!
187 steering wheel lock defective
188 steering wheel lock defective
189 steering wheel lock defective
190 steering wheel lock defective
191 nothing
192 Initialise Tyre Monitor (RDC)
193 Emergency exit fault!
194 Emergency exit  fault
195 park distance control
196 park distance control
197 emergency exit fault
198 nothing
199 nothing
200 nothing
201 automatic hold. apply the brakes
202 automatic hold. apply the brakes
203 transmission in position N!
204 chassis. drive Moderately
205 next press of button starts engine
206 next press of button starts engine
207 nothing
208 nothing
209 remote key inside car
210 parking brake failure!
211 parking brake failure!
212 Engine oil pressure?
213 Charging fault
214 nothing
215 DSC
216 Fuel supply. Drive Moderately
217 hold remote control against start button!
218 hold remote control against start button!
219 hold remote control against start button!
220 Increased battery discharge
221 gas alarm! leave the area
222 gas alarm! leave the area
223 electral fault! drive Moderately 
224 Insulation fault
225 Windscreen unlocked
226 fire exting fault!
227 fire exting fault
228 windscreen unlocked
229 charge battery
230 charge battery
231 lighting system. stop carefully
232 Protection system fault
233 communication fault
234 assault alarm fault
235 assault alarm fault
236 driving stabilisation drive Moderately
237 driving stabilisation failure
238 Driving stabilisation failure
239 parking brake only partially available
240 parking brake failure
241 parking brake fail/partially available
242 parking brake only partially available
243 parking brake failure/partially available
244 to engage gear, press brake
245 driving comfort restricted
246 nothing?
247 battery monitoring fault
248 nothing?
249 nothing
250 press brake to engage gear
251 engaging gearbox position P!
252 nothing?
253 Handbrake on
254 transmission fault! Drive Moderately
255 transmission fault! drive Moderately
```

# Credits
-jas3r
