# Travel Preferences

    public class CuisinePreferences : PersonalPreferenceProfile
    {
        public PreferenceSet Enjoy { get; } =
        {
            Cities:
            {
                South Padre Island,
                Boston,
                Seattle,
                New Orleans,
                Chicago,
                St. Louis,
                Denver
            },

            Resorts-Accomodations:
            {
                Margaritaville,
                Beale Mansion,
                Turkey Run Inn,
                Great Rivers,
                Terre Haute Casino,
            },
        };

        public PreferenceSet BucketList.ordered { get; } =
        {
            Cities:
            {
                "Pau, FR",
                "Silsden, UK",
                "Doncaster, UK",
                "Kaunas, LT",
                "Camana Bay, CYM",
                "Lereci, IT",
                Amsterdam,
                "Pictou, NS, CA",
                "Macinac Island,"
                Vancouver,
                "Sochi, RU",
                "Rekjavik, IS",
                Toronto,
                Budapest,
                Vienna
                "Chiba, JP",
                Las Vegas,
                Hong Kong,
                Rio,
                Copenhagen,
            }

            Restorts-Accomodations:
            {
                "Viešbutis Kaunas",
                "Novotel Pau Pyrénées",
                "Hotel Shelley e delle Palme",
                "Swissôtel Resort Сочи Камелия",
                "ONE GT Grand Cayman",

            }

            Experiences:
            {
                Cruise,
                "Ski Lodge",
                "Writer's Cabin",
            }
        }    

        enum Preferred
        {
            Ocean View,
            Palm Trees,
            Resort Atmosphere,
            Local Cuisine,
            Local Culture,
            Balconies,
            Museums,
            Historical Sites,
            Architecture,
            Subculture,
            Local Drinking Establishments,
            Walkable Neighborhood            
        }

        enum Disfavored
        {
            Many Children,
            Touristy,
            "Roughing it",
            Campgrounds
        }
    }
