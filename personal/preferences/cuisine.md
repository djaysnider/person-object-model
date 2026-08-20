# Cusisine Preferences

    public class CuisinePreferences : PersonalPreferenceProfile
    {
        public PreferenceSet Preferred { get; } =
        {
            Indian:
            {
                Vindaloo,
                Tandoori,
                TikkaMasala,
                PalakPaneer,
                GarlicNaan,
                Pakora
            },

            Chinese.Americanized:
            {
                GeneralTsosChicken,
                BourbonChicken,
                MongolianPork,
                SzechuanBeef,
                KungPaoShrimp,
                CrabRangoon,
                HotAndSourSoup,
                HappyFamily
            },

            Sushi:
            {
                PhillyRoll,
                EelNigiri,
                RainbowRoll,
                FishersRoll,
                DragonRoll,
                SpicySpiderRoll
            }
        };


        public PreferenceSet Approved { get; } =
        {
            Standbys:
            {
                BarbecuedPorkSteaks,
                ChicagoHotDog,
                PorkTenderloin,
                NewYorkStrip,
            }

            Mexican:
            {
                ChorizoTorta,
                HuevosRancheros,
                FajitasCozumel,
                SeafoodEnchilada,
                Tostaguac,
                Chalupa,
                ChileRelleno
            }
        };


        public BeveragePreferences Beverages { get; } = new()
        {
            Alcoholic =
            {
                Beer:
                {
                    BuschLight,
                    BudLight,
                    BelhavenScottishAle,
                    KonaBigWave,
                    SunKingPachanga,
                    ThreeFloydsAlphaKing,
                    Modelo,
                    CraftLagers
                },

                Wine:
                {
                    Merlot,
                    Malbec,
                    Cabernet,
                    PinotNoir,
                    LambruscoReggiano
                }
            },

            NonAlcoholic =
            {
                IcedTea(Sweetness.Medium),
                TimHortonsCoffee,
                PistachioLatte,
                DietCoke,
                DietDrPepper
            }

            Untested =
            {
                Moussaka,
                Bouillabaisse,
                Borscht,
                Šaltibarščiai,
                Cepelinai,
                Gravlax,
                Kjötsúpa
            },

            Failed =
            {
                TakoSashimi
            }

        };


        public PreparationSkill Cooking { get; } = new()
        {
            Mastered =
            {
                Lasagna,
                SalmonWellington,
                FrenchBread,
                StuffedMushrooms,
                EnchiladasCancun,
                Jambalaya
            }
        }

        Public IReadOnlySet<Food> JudgedOverSubjectively { get; } =
        {
            StLouisButterCake,
            CoconutCreamPie,
            CremeHorns,
            Lasagna,
            PotatoSalad
        };


        public IReadOnlySet<ConsumptionWarning> KnownSideEffects { get; } =
        {
            new(RawOysters, Risk.Unpleasant),
            new(Tomato, Risk.Unpleasant)
            {
                Condition = TimeOfDay > 20:00
            }
        };

       Instance Pizza:
        {
            Preference = Standby,
            Preparation = AboveAverage,
            JudgmentBias = High,
            PreferredStyle = {"Chicago","TavernStyle","Sicilian"},
            PreferredSource = {"Gino's","Georgio's","Ale Emporium","Curry Pizza","Monicals","Donatos","Chicago Pizza"}
            AnchovyRequired = true,
            BlackOliveRequired = preferable,
            MushroomRequired = preferable,
            MeatRequired = any,
            ArtisanPizza = someexceptions,
            PineappleAsIngredient = tolerated
        }

       Instance Lasagna:
        {
            Preference = Preferred,
            Preparation = Mastered,
            JudgmentBias = Extreme,
            RicottaRequired = true,
            CottageCheeseSubstitution = Heresy
        }

        Instance TakoSashimi:
        {
            Preference = Failed,
            Opinion = Inedible,
            Attempts = 2,
            RetryPolicy = Never,
            PostMortemAvailable = true
        }

        enum Preference
        {
            Optimal,
            Preferred,
            Approved,
            Tolerated,
            Situational,
            Untested,
            Pessimal,
            AbsolutelyNot
        }

        enum Confidence
        {
            Tentative,
            Experienced,
            StronglyHeld,
            IrrationallyCertain,
            WillArgueOverDinner
        }

        enum RetryPolicy
        {
            Immediately,
            Eventually,
            IfSomeoneElseIsPaying,
            UnderDuress,
            Never
        }
    }
