# Hotel_System
#powerbi #datavisualisation #mssqlserver

with hotels as (
select*from dbo.['2018$']
union
select*from dbo.['2019$']
union
select*from dbo.['2020$'])

select*from hotels
left join dbo.market_segment$
on hotels.market_segment = market_segment$.market_segment
left join dbo.meal_cost$
on meal_cost$.meal = hotels.meal


--select 
--arrival_date_year,
--hotel type,
--sum((stays_in_week_nights+stays_in_weekend_nights)* adr) as revenue 
--from hotels
--group by arrival_date_year,hotel
--select*from dbo.market_segment$

<img width="662" alt="HotelSystem" src="https://user-images.githubusercontent.com/60243643/232173964-a54fdb8e-679c-4f94-97b2-c665aecac655.png">




[HotelSystem (2020).pdf](https://github.com/chichi-pixel/Hotel_System/files/11237901/HotelSystem.2020.pdf)



[HotelSystem.pdf](https://github.com/chichi-pixel/Hotel_System/files/11237903/HotelSystem.pdf)






