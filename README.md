Request Flow-->
1.Controller receives employee or attendance data.
2.Controller calls EmployeeService.createEmployee(employee) or relevant service method.
3.Service Layer processes business logic.
4.Repository Layer saves/fetches data from the database.
5.Returns ApiResponse with success or error status.

DTO Usage

DTOs act as data carriers at different stages of the request–response cycle:
AttendanceRequest → Used when sending input from the client
AttendanceResponse → Used when sending success response back
AttendanceSummaryDTO → Full summary response with nested data
DailyAttendanceDTO → Represents one day’s attendance
AttendanceRecordDTO → Represents a single punch (In/Out record)
ApiResponse → Standard wrapper for all API responses
