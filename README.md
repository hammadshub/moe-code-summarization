                  RESEARCH QUESTION
                         │
                         ▼
       Can specialized experts improve
             code summarization?
                         │
             ┌───────────┴───────────┐
             │                       │
             ▼                       ▼
        DENSE MODEL                 MoE
       CodeT5+ 220M                 │
             │                      ▼
       All training data          Gate
             │                 ┌────┴────┐
             │                 ▼         ▼
             │              Method    Function
             │              Expert     Expert
             │                 │         │
             │                 └────┬────┘
             │                      │
             ▼                      ▼
         BASELINE                 MOE
             │                      │
             └──────────┬───────────┘
                        ▼
                    COMPARE
                        │
                        ▼
              MoE performed worse
                        │
                        ▼
             WHY?
                        │
             ┌──────────┴──────────┐
             ▼                     ▼
        Less data per          Majority category
           expert              already benefited
             │                     │
             └──────────┬──────────┘
                        ▼
             Specialization alone
             isn't automatically useful
