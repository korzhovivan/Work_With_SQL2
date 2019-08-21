--111111111111111111111111111111111111111111

--Declare @X int, @Cnt int, @number int

--Set @X=1
--Set @Cnt=1

--Set @number = 5

--While (@Cnt<=@number)
--begin
-- Select @X=@X*@Cnt
-- Select @Cnt=@Cnt+1
--end

--Select Result=@X

--2222222222222222222222222222222222222222222

--CREATE PROCEDURE ProductSummary AS
--BEGIN
--    SELECT DATEADD(yy, 2, Books.DateOfPublishing)
--	FROM Books
--END;

--exec ProductSummary

--333333333333333333333333333333333333333333333

--CREATE PROCEDURE FindAuthorInfo
--	@country nvarchar(20)
--AS
--BEGIN
--    SELECT Authors.FirstName, Authors.LastName, Country.NameCountry
--	from Authors,Country
--	where Authors.ID_COUNTRY = Country.ID_COUNTRY
--	and Country.NameCountry = @country
--END;
--exec FindAuthorInfo 'USA'

--444444444444444444444444444444444444444444444

--create procedure AvgPages
--	@firstDate date,
--	@secondDate date
--as
--	select avg(Books.Pages) 
--	from Books
--	where  Books.DateOfPublishing between @firstDate and @secondDate

--exec AvgPages '1990-07-01', '2010-12-31'

--555555555555555555555555555555555555555555555555


--create procedure ShowBookInfo
--	@year int
--as
--	select Books.NameBook, Books.Price, Books.DateOfPublishing
--	from Books
--	where year(Books.DateOfPublishing) = @year 

--exec ShowBookInfo 2001