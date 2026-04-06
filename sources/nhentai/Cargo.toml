use aidoku::{
    error::Result,
    prelude::*,
    std::{Vec, String},
    Manga, MangaPageResult, Listing, Chapter, Page, Filter,
};

#[get_manga_list]
fn get_manga_list(_filters: Vec<Filter>, _page: i32) -> Result<MangaPageResult> {
    Ok(MangaPageResult {
        manga: Vec::new(),
        has_more: false,
    })
}

#[get_manga_details]
fn get_manga_details(_id: String) -> Result<Manga> {
    Err(aidoku::error::AidokuError { t: aidoku::error::AidokuErrorKind::Unimplemented })
}

#[get_chapter_list]
fn get_chapter_list(_id: String) -> Result<Vec<Chapter>> {
    Ok(Vec::new())
}

#[get_page_list]
fn get_page_list(_manga_id: String, _chapter_id: String) -> Result<Vec<Page>> {
    Ok(Vec::new())
}

#[modify_image_request]
fn modify_image_request(_request: aidoku::std::net::Request) {}

#[handle_url]
fn handle_url(_url: String) -> Result<DeepLink> {
    Err(aidoku::error::AidokuError { t: aidoku::error::AidokuErrorKind::Unimplemented })
}
