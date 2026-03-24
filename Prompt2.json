You are given some text describing a military ship. Analyze it and extract the following features.
Each attribute is encoded as a number. Combine values if needed (e.g., elevator locations 1 and 2 become 12).
At the end, output a single Python-style list, and only the list (no explanation, no extra text).
Field order:
1. deck_type: 0 [unknown], 1 [full-length deck], 2 [angled deck]
2. island_location: 0 [unknown], 1 [forward starboard mid], 2 [mid starboard], 3 [aft starboard mid], 4 [dual islands]
3. estimated_length_m: numeric value or 0 if unknown
4. estimated_width_m: numeric value or 0 if unknown
5. hull_number_location: 0 [unknown], 1 [bow], 2 [stern], 3 [island]
6. hull_number: 0 [unknown] or actual number
7. number_of_elevators: 0 [unknown] or actual count
8. elevator_location: 0 [unknown], 1 [starboard forward], 2 [starboard aft], 3 [port center], 4 [starboard center]; combinations like 1 and 2 → 12
9. helicopter_platform_distribution: 0 [unknown], 1 [concentrated], 2 [dispersed]
10. embarked_aircraft_model: 0 [unknown], 1 [AV-8B Harrier II], 2 [CH-46/CH-53-type helicopters], 3 [E-2 Hawkeye], 4 [F-14 Tomcat],
    5 [F-4 Phantom (museum static)], 6 [F/A-18 Hornet], 7 [Harrier AV-8S or SH-60B (cannot confirm precisely)], 8 [J-15],
    9 [MV-22 Osprey], 10 [MiG-29K], 11 [SH-3 Sea King], 12 [SH-60K], 13 [SH-60K or unknown], 14 [Sea Harrier], 15 [Su-33],
    16 [UH-60-type helicopters], 17 [mixed museum aircraft (e.g., F-14)], 18 [mixed museum aircraft (e.g., F/A-18, A-4, F-14)],
    19 [mixed museum display (e.g., F/A-18, F-14, A-4)], 20 [static museum aircraft (e.g., F/A-18, F-14)]
11. visibility: 1 [good], 2 [moderate], 3 [poor]
12. surrounding_facilities: 0 [unknown], 1 [dry dock], 2 [naval base], 3 [ship exhibition], 4 [open sea]
Example input (for your understanding only):
{
  "deck_type": 1,
  "island_location": 2,
  "estimated_length_m": 255,
  "estimated_width_m": 32,
  "hull_number_location": 0,
  "hull_number": 0,
  "number_of_elevators": 2,
  "elevator_location": 12,
  "helicopter_platform_distribution": 2,
  "embarked_aircraft_model": 0,
  "visibility": 1,
  "surrounding_facilities": 2
}
Example output:
[1, 2, 255, 32, 0, 0, 2, 12, 2, 0, 1, 2]
Your task: Given a text describing a ship, extract and output the list as above.
