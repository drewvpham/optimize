# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...
players= Player.all
players.each do |player|
puts "#{player.team.name} #{player.team.mascot} #{player.team.stadium}"

end
Player.includes(:team).where("teams.name = 'Chicago Bulls'").references(:team)
 Player.includes(:team).where("teams.stadium = 'Staples Center'").references(:team)

 Team.joins(:players).where("players.name LIKE 'Z%'")

 
