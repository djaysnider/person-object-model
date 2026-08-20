# Dependencies

    public class Dependencies : PersonalDependecyProfile
    (
        public DependecySet Work { get; } =
        {
            Work:
            {
                Lighting = {"dim","non-flourescent"},
                Music = {"jazz-hop","lo-fi","shoegaze"},
                Conversation = minimal,
                Walls = required,
                People = sparse,
                Monitors.minimum = 2,
                Deskspace.minimum = 16sqft,
                Coffee = free,
            }

            Sleep:
            {
                Lighting = dark,
                Music.weekday = {"Soma FM Darkzone","KCSM","BBC Radio 3"},
                Music.weekend = {"AM America Old Time Radio","BBC Radio 4"},
                Fan = on,
                Window = open,
                Mattress = firm,
                Pillow = feather,
                Pillow.cout = 2,
            }

            Writing:
            {
                Lighting = {"daylight","non-flourescent"},
                Music = {"dnb","ambient","specialized by work"},
                Conversation = none,
                Outline = {"present","ignored"},
                SprintTime = {25, 60},
                PublicSpace = prefered,
                Beverage = {"coffee","tea","wine"},
                Device = {"laptop","tablet"},
            }
        }
    )
