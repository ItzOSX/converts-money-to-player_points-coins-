# &b&lConverts-money-to-player_points-coins-
A simple and functional skript that can converts eco-money to player_points that can be used in coinshops
-----------------------------------------------------------------------------------------------------------------------------------------
command /convertpoints:
    description: Convert 1,000,000 money to 500 PlayerPoints
    trigger:
        if player's balance >= 1000000:
            remove 1000000 from player's balance
            execute console command "playerpoints:p give %player% 500"
            send "&c&lYou have successfully converted 1,000,000 money into 500 PlayerPoints!"
        else:
            send "&b&lYou don't have enough money to convert!"
