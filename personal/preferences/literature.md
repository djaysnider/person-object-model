# Literary Preferences

    public class Books : PersonalPreferenceProfile
    {
        public PreferenceSet ByGenre { get; } =
        {
            Thriller:
            {
                Robert Ludlum,
                Eric Van Lustbader,
                Jack Higgins,
                Tom Clancy,
                Clive Cussler
            },

            Science Fiction:
            {
                Arthur C.Clarke,
                Isaac Asimov,
                William Gibson,
                David Weber,
                David Brin,
                Elizabeth Moon,
                William Tedford,
                Steven Baxter

            },

            Mystery:
            {
                Gregory McDonald,
                Travis McGee,
                Lawrence Block,
                Dashiel Hammet,
                Donald Hamilton
            }

            Literary:
            {
                Alain Robbe-Grillet,
                Franz Khafka,
                Jack London,
                Kurt Vonnegut,
                Jack Kerouac,
                Haruki Murakami
            }

            Humor:
            {
                Douglas Adams,
                Chuck Klosterman,
                John Hodgman,
                David Mitchell,
                Nick Spalding
            }

            Poetry:
            {
                Bob Holman,
                Nicole Blackman,
                Hal Sirowitz,
                Maggie Estep,
                M. Doughty,
                Allen Ginsberg                
            }
        };

        public PreferenceSet ByTitle { get; }
        {
            Pattern Recognition,
            Death of a Citizen,
            Rendezvous with Rama,
            Manifold: Time,
            Soft Maniacs,
            Martin Eden,
            Neuromancer,
            Flight of Eagles,
            The Areas of My Expertise,
            Sex, Drugs, and Cocoa Puffs,
            Confess, Fletch,
            Grumpy Old Rock Star,
            The End of Eternity
        }

        Public PreferenceSet BySeries { get; }
        {
            The Hitchhiker's Guide to the Galaxy,
            Fletch,
            Matt Helm,
            Jack Ryan,
            Paul Chavasse,
            Liam Devlin,
            The Sprawl,
            Blue Ant,
            Rama,
            Dune,
            Foundation,
            Guardians of the Flame,
            The Shadow
        }

        Public PreferenceSet WorstBooks { get; }
        {
            I Hope They Serve Beer in Hell,
            Bandwidth,
            The Last Days of August,
            Soldier of the Legion,
            Your Favorite Band Cannot Save You,
            Critical Failures,
            Taipei,
            Veronica,
            Gilead,
            The Sound and the Fury            
        }
    }