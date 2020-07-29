--
-- PostgreSQL database dump
--

-- Dumped from database version 12.1
-- Dumped by pg_dump version 12.1

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

SET default_tablespace = '';

SET default_table_access_method = heap;

--
-- Name: Artist; Type: TABLE; Schema: public; Owner: connorlynch
--

CREATE TABLE public."Artist" (
    id integer NOT NULL,
    name character varying(120),
    city character varying(120),
    state character varying(120),
    address character varying(120),
    phone character varying(120),
    genres character varying[],
    image_link character varying(500),
    website character varying(120),
    facebook_link character varying(120),
    created_at timestamp without time zone,
    updated_at timestamp without time zone,
    seeking_venue boolean NOT NULL,
    seeking_description character varying(120)
);


ALTER TABLE public."Artist" OWNER TO connorlynch;

--
-- Name: Artist_id_seq; Type: SEQUENCE; Schema: public; Owner: connorlynch
--

CREATE SEQUENCE public."Artist_id_seq"
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public."Artist_id_seq" OWNER TO connorlynch;

--
-- Name: Artist_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: connorlynch
--

ALTER SEQUENCE public."Artist_id_seq" OWNED BY public."Artist".id;


--
-- Name: Show; Type: TABLE; Schema: public; Owner: connorlynch
--

CREATE TABLE public."Show" (
    id integer NOT NULL,
    artist_id integer,
    venue_id integer,
    start_time timestamp without time zone NOT NULL
);


ALTER TABLE public."Show" OWNER TO connorlynch;

--
-- Name: Show_id_seq; Type: SEQUENCE; Schema: public; Owner: connorlynch
--

CREATE SEQUENCE public."Show_id_seq"
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public."Show_id_seq" OWNER TO connorlynch;

--
-- Name: Show_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: connorlynch
--

ALTER SEQUENCE public."Show_id_seq" OWNED BY public."Show".id;


--
-- Name: Venue; Type: TABLE; Schema: public; Owner: connorlynch
--

CREATE TABLE public."Venue" (
    id integer NOT NULL,
    name character varying(120),
    city character varying(120),
    state character varying(120),
    address character varying(120),
    phone character varying(120),
    genres character varying[],
    image_link character varying(500),
    website character varying(120),
    facebook_link character varying(120),
    created_at timestamp without time zone,
    updated_at timestamp without time zone,
    seeking_talent boolean NOT NULL,
    seeking_description character varying(120)
);


ALTER TABLE public."Venue" OWNER TO connorlynch;

--
-- Name: Venue_id_seq; Type: SEQUENCE; Schema: public; Owner: connorlynch
--

CREATE SEQUENCE public."Venue_id_seq"
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public."Venue_id_seq" OWNER TO connorlynch;

--
-- Name: Venue_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: connorlynch
--

ALTER SEQUENCE public."Venue_id_seq" OWNED BY public."Venue".id;


--
-- Name: alembic_version; Type: TABLE; Schema: public; Owner: connorlynch
--

CREATE TABLE public.alembic_version (
    version_num character varying(32) NOT NULL
);


ALTER TABLE public.alembic_version OWNER TO connorlynch;

--
-- Name: Artist id; Type: DEFAULT; Schema: public; Owner: connorlynch
--

ALTER TABLE ONLY public."Artist" ALTER COLUMN id SET DEFAULT nextval('public."Artist_id_seq"'::regclass);


--
-- Name: Show id; Type: DEFAULT; Schema: public; Owner: connorlynch
--

ALTER TABLE ONLY public."Show" ALTER COLUMN id SET DEFAULT nextval('public."Show_id_seq"'::regclass);


--
-- Name: Venue id; Type: DEFAULT; Schema: public; Owner: connorlynch
--

ALTER TABLE ONLY public."Venue" ALTER COLUMN id SET DEFAULT nextval('public."Venue_id_seq"'::regclass);


--
-- Data for Name: Artist; Type: TABLE DATA; Schema: public; Owner: connorlynch
--

COPY public."Artist" (id, name, city, state, address, phone, genres, image_link, website, facebook_link, created_at, updated_at, seeking_venue, seeking_description) FROM stdin;
3	Tahirah Banks	Houston	TX	\N	2644764466	{Alternative,Blues,Classical}	https://cdn.vox-cdn.com/thumbor/e9LHdmupeM1u0QLV0wMdB8VqfqQ=/0x0:2841x1171/920x613/filters:focal(1807x402:2261x856):format(webp)/cdn.vox-cdn.com/uploads/chorus_image/image/65958141/Screen_Shot_2019_07_18_at_4.16.52_PM.0.png	\N	https://www.facebook.com/profile.php?id=100011291887654	2020-07-15 21:14:39.667201	2020-07-15 21:14:39.667201	f	
5	Ariel Bushay	New York City	NY	\N	2644764466	{Alternative,Blues,Classical,Country}	https://cdn.vox-cdn.com/thumbor/e9LHdmupeM1u0QLV0wMdB8VqfqQ=/0x0:2841x1171/920x613/filters:focal(1807x402:2261x856):format(webp)/cdn.vox-cdn.com/uploads/chorus_image/image/65958141/Screen_Shot_2019_07_18_at_4.16.52_PM.0.png	\N	https://www.facebook.com/profile.php?id=100011291887654	2020-07-15 21:15:44.668277	2020-07-15 21:15:44.668277	t	Look for a place to play!
6	Olaide Banks	Morgantown	WV	\N	3462709666	{Classical,Country}	https://cdn.vox-cdn.com/thumbor/e9LHdmupeM1u0QLV0wMdB8VqfqQ=/0x0:2841x1171/920x613/filters:focal(1807x402:2261x856):format(webp)/cdn.vox-cdn.com/uploads/chorus_image/image/65958141/Screen_Shot_2019_07_18_at_4.16.52_PM.0.png	\N	https://www.facebook.com/profile.php?id=100011291887654	2020-07-15 21:16:16.659363	2020-07-15 21:16:16.659363	f	
4	Kordell Smith	Houston	TX	\N	2644764466	{Alternative,Blues,Classical,Country}	https://cdn.vox-cdn.com/thumbor/e9LHdmupeM1u0QLV0wMdB8VqfqQ=/0x0:2841x1171/920x613/filters:focal(1807x402:2261x856):format(webp)/cdn.vox-cdn.com/uploads/chorus_image/image/65958141/Screen_Shot_2019_07_18_at_4.16.52_PM.0.png	\N	https://www.facebook.com/profile.php?id=100011291887654	2020-07-15 21:15:06.446491	2020-07-15 21:15:06.446491	f	
\.


--
-- Data for Name: Show; Type: TABLE DATA; Schema: public; Owner: connorlynch
--

COPY public."Show" (id, artist_id, venue_id, start_time) FROM stdin;
4	6	1	2020-07-15 21:18:52
5	3	2	2020-07-16 21:18:52
\.


--
-- Data for Name: Venue; Type: TABLE DATA; Schema: public; Owner: connorlynch
--

COPY public."Venue" (id, name, city, state, address, phone, genres, image_link, website, facebook_link, created_at, updated_at, seeking_talent, seeking_description) FROM stdin;
1	The Burberry Tree	Houston	TX	11510 Ocotillo Dr	2644764466	{Alternative,Blues,Classical}	https://cdn.vox-cdn.com/thumbor/e9LHdmupeM1u0QLV0wMdB8VqfqQ=/0x0:2841x1171/920x613/filters:focal(1807x402:2261x856):format(webp)/cdn.vox-cdn.com/uploads/chorus_image/image/65958141/Screen_Shot_2019_07_18_at_4.16.52_PM.0.png	http://www.acme.com	https://www.facebook.com/profile.php?id=100011291887654	2020-07-13 23:35:56.02319	2020-07-13 23:35:56.02319	t	We're looking for young hip artists to jass up the place.
2	The Big Apple	Houston	TX	11510 Ocotillo Dr	2644764466	{Country,Electronic,Folk}	https://cdn.vox-cdn.com/thumbor/e9LHdmupeM1u0QLV0wMdB8VqfqQ=/0x0:2841x1171/920x613/filters:focal(1807x402:2261x856):format(webp)/cdn.vox-cdn.com/uploads/chorus_image/image/65958141/Screen_Shot_2019_07_18_at_4.16.52_PM.0.png	www.whythoughtful.com	https://www.facebook.com/profile.php?id=100011291887654	2020-07-15 20:51:17.714427	2020-07-15 20:51:17.714427	t	Just a test
\.


--
-- Data for Name: alembic_version; Type: TABLE DATA; Schema: public; Owner: connorlynch
--

COPY public.alembic_version (version_num) FROM stdin;
db73d97e4478
\.


--
-- Name: Artist_id_seq; Type: SEQUENCE SET; Schema: public; Owner: connorlynch
--

SELECT pg_catalog.setval('public."Artist_id_seq"', 6, true);


--
-- Name: Show_id_seq; Type: SEQUENCE SET; Schema: public; Owner: connorlynch
--

SELECT pg_catalog.setval('public."Show_id_seq"', 5, true);


--
-- Name: Venue_id_seq; Type: SEQUENCE SET; Schema: public; Owner: connorlynch
--

SELECT pg_catalog.setval('public."Venue_id_seq"', 2, true);


--
-- Name: Artist Artist_pkey; Type: CONSTRAINT; Schema: public; Owner: connorlynch
--

ALTER TABLE ONLY public."Artist"
    ADD CONSTRAINT "Artist_pkey" PRIMARY KEY (id);


--
-- Name: Show Show_pkey; Type: CONSTRAINT; Schema: public; Owner: connorlynch
--

ALTER TABLE ONLY public."Show"
    ADD CONSTRAINT "Show_pkey" PRIMARY KEY (id);


--
-- Name: Venue Venue_pkey; Type: CONSTRAINT; Schema: public; Owner: connorlynch
--

ALTER TABLE ONLY public."Venue"
    ADD CONSTRAINT "Venue_pkey" PRIMARY KEY (id);


--
-- Name: alembic_version alembic_version_pkc; Type: CONSTRAINT; Schema: public; Owner: connorlynch
--

ALTER TABLE ONLY public.alembic_version
    ADD CONSTRAINT alembic_version_pkc PRIMARY KEY (version_num);


--
-- Name: Show Show_artist_id_fkey; Type: FK CONSTRAINT; Schema: public; Owner: connorlynch
--

ALTER TABLE ONLY public."Show"
    ADD CONSTRAINT "Show_artist_id_fkey" FOREIGN KEY (artist_id) REFERENCES public."Artist"(id) ON DELETE CASCADE;


--
-- Name: Show Show_venue_id_fkey; Type: FK CONSTRAINT; Schema: public; Owner: connorlynch
--

ALTER TABLE ONLY public."Show"
    ADD CONSTRAINT "Show_venue_id_fkey" FOREIGN KEY (venue_id) REFERENCES public."Venue"(id) ON DELETE CASCADE;


--
-- PostgreSQL database dump complete
--

