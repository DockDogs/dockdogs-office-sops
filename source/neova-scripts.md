Neova Checks
===========================

## Complimentary Access Checks


* Step 1( check whether team is member or not ):                  
`
    SELECT `t`.`id` AS `not_members_id`FROM `teams` `t` WHERE t.is_archived = "N" AND (( t.id NOT IN 
                    (
                        SELECT tms.team_id
                        FROM teams_membership_status AS tms
                        WHERE tms.team_id IN (14411 )
                        AND tms.seasons = 20
                    )
                )
                AND
                (
                    t.id IN
                    (
                        SELECT teams_id
                        FROM teams_waves_registration AS twr
                        WHERE twr.teams_id in (14411 ) AND twr.season_id = 20  AND twr.admin_type =3
                        group by teams_id having count(DISTINCT twr.transaction_token) >= 2 
                    )
                )
        ) AND t.id IN( 14411 )


* Step 2 ( then check for the complementary transaction for non member team id ): 
````
                                         SELECT *  FROM `teams_waves_registration` WHERE `teams_id` = 14411 AND `admin_type` = 3 AND `season_id` = 20 group by transaction_token;
````
                       
