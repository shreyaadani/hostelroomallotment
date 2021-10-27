## [please download the war file to get the entire project with all required packages and binaries]


# hostelroomalloctment
hostel room allotment based on the room type and no of roomates choosen.

This project required Database created in postgresql and src need to be changed for connecting database server if it is not on localhost.
Required tables are as below
!> Table Roomdetails
-- Table: public.roomdetails

-- DROP TABLE public.roomdetails;

CREATE TABLE public.roomdetails
(
    roomno integer,
    bedtype integer,
    floor integer,
    buildingno integer,
    hosteltype character varying(5) COLLATE pg_catalog."default",
    allocated boolean
)

2. Table student
-- Table: public.student

-- DROP TABLE public.student;

CREATE TABLE public.student
(
    name character varying(60) COLLATE pg_catalog."default" NOT NULL,
    password character varying(12) COLLATE pg_catalog."default",
    CONSTRAINT student_pkey PRIMARY KEY (name)
)
3. Table studentinfo
-- Table: public.studentinfo

-- DROP TABLE public.studentinfo;

CREATE TABLE public.studentinfo
(
    name character varying COLLATE pg_catalog."default",
    password character varying COLLATE pg_catalog."default",
    registrationno character varying COLLATE pg_catalog."default",
    hostelindex integer,
    selectiondone boolean,
    branch character varying COLLATE pg_catalog."default",
    roomis integer
)

Please create and fill inital data for proper implementation of this project.
